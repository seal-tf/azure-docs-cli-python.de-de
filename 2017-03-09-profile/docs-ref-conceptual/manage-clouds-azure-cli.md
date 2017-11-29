---
title: Verwalten mehrerer Clouds mit der Azure CLI 2.0
description: "Die Azure CLI 2.0 ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei verschiedenen Clouds."
keywords: Azure CLI 2.0, Azure, Clouds, Datencenter, Regierung, Region, China, Deutschland
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: cb470d179daf7cb4ecf535903adb12071602034e
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="68ea0-104">Verwalten mehrerer Clouds mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="68ea0-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="68ea0-105">Wenn Sie regionsübergreifend arbeiten oder [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/) verwenden, müssen Sie möglicherweise mehrere Clouds verwenden.</span><span class="sxs-lookup"><span data-stu-id="68ea0-105">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="68ea0-106">Hierzu stellt Ihnen Microsoft Clouds zur Verfügung, die mit regionalen Gesetzen in Einklang stehen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-106">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="68ea0-107">In diesem Artikel erfahren Sie, wie Sie Informationen zu Clouds abrufen, die für Ihr Konto verfügbar sind, wie Sie die aktuelle Cloud ändern und wie Sie neue Clouds für die Verwendung mit Azure Stack registrieren bzw. die Registrierung aufheben.</span><span class="sxs-lookup"><span data-stu-id="68ea0-107">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="68ea0-108">Auflisten von Clouds</span><span class="sxs-lookup"><span data-stu-id="68ea0-108">Listing clouds</span></span>

<span data-ttu-id="68ea0-109">Die verfügbaren Clouds können mit dem Befehl [cloud list](/cli/azure/cloud#list) aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="68ea0-109">You can list available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="68ea0-110">So erfahren Sie, welche Cloud derzeit aktiv ist, und erhalten Informationen zum aktuellen Profil, zu regionalen Suffixen und zu Hostnamen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-110">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="68ea0-111">Gehen Sie wie folgt vor, um die aktive Cloud und eine Liste mit allen verfügbaren Clouds abzurufen:</span><span class="sxs-lookup"><span data-stu-id="68ea0-111">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

<span data-ttu-id="68ea0-112">Für die derzeit aktive Cloud ist in der Spalte `IsActive` der Wert `True` angegeben.</span><span class="sxs-lookup"><span data-stu-id="68ea0-112">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="68ea0-113">Es kann immer nur eine Cloud aktiv sein.</span><span class="sxs-lookup"><span data-stu-id="68ea0-113">Only one cloud can be active at any time.</span></span> <span data-ttu-id="68ea0-114">Ausführlichere Informationen zu einer Cloud (einschließlich der Endpunkte, die sie für Azure-Dienste verwendet) erhalten Sie mit dem Befehl `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="68ea0-114">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a><span data-ttu-id="68ea0-115">Wechseln der aktiven Cloud</span><span class="sxs-lookup"><span data-stu-id="68ea0-115">Switching the active cloud</span></span>

<span data-ttu-id="68ea0-116">Führen Sie zum Wechseln der aktiven Cloud den Befehl [cloud set](/cli/azure/cloud#set) aus.</span><span class="sxs-lookup"><span data-stu-id="68ea0-116">To switch the currently active cloud, run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="68ea0-117">Dieser Befehl erfordert ein Argument: den Namen der Cloud.</span><span class="sxs-lookup"><span data-stu-id="68ea0-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="68ea0-118">Sollte die Authentifizierung für die aktivierte Cloud abgelaufen sein, müssen Sie sich erneut authentifizieren, bevor Sie weitere CLI-Aufgaben ausführen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="68ea0-119">Beim erstmaligen Wechsel zu der neuen Cloud muss auch das aktive Abonnement festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="68ea0-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="68ea0-120">Anleitungen zur Authentifizierung finden Sie unter [Log in with Azure CLI 2.0](authenticate-azure-cli.md) (Anmelden bei der Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="68ea0-120">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="68ea0-121">Weitere Informationen zur Abonnementverwaltung finden Sie unter [Verwalten mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="68ea0-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="68ea0-122">Registrieren einer Cloud</span><span class="sxs-lookup"><span data-stu-id="68ea0-122">Register a cloud</span></span>

<span data-ttu-id="68ea0-123">Registrieren Sie eine neue Cloud, wenn Sie über eigene Endpunkte für Azure Stack verfügen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="68ea0-124">Eine Cloud wird mit dem Befehl [cloud register](/cli/azure/cloud#register) erstellt.</span><span class="sxs-lookup"><span data-stu-id="68ea0-124">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="68ea0-125">Dieser Befehl erfordert einen Namen und einen Satz von Funktionen mit den dazugehörigen Endpunkten.</span><span class="sxs-lookup"><span data-stu-id="68ea0-125">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="68ea0-126">Informationen zum Registrieren einer Cloud für die Verwendung mit Azure Stack finden Sie unter [Installieren und Konfigurieren der CLI für die Verwendung mit Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="68ea0-126">To learn how to register a cloud for use with Azure Stack, see [Install and configure CLI for use with Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span></span>  

<span data-ttu-id="68ea0-127">Für China, US Government oder deutsche Regionen müssen Sie Ihre eigene Cloud nicht registrieren.</span><span class="sxs-lookup"><span data-stu-id="68ea0-127">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="68ea0-128">Diese werden von Microsoft verwaltet und sind standardmäßig verfügbar.</span><span class="sxs-lookup"><span data-stu-id="68ea0-128">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="68ea0-129">Weitere Informationen zu allen verfügbaren Endpunkteinstellungen finden Sie in der [Dokumentation für `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span><span class="sxs-lookup"><span data-stu-id="68ea0-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span></span>

<span data-ttu-id="68ea0-130">Durch Registrieren einer Cloud wird nicht automatisch zu dieser Cloud gewechselt.</span><span class="sxs-lookup"><span data-stu-id="68ea0-130">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="68ea0-131">Wählen Sie die neu erstellte Cloud wie weiter oben beschrieben mithilfe des Befehls `az cloud set` aus.</span><span class="sxs-lookup"><span data-stu-id="68ea0-131">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="68ea0-132">Aktualisieren einer vorhandenen Cloud</span><span class="sxs-lookup"><span data-stu-id="68ea0-132">Update an existing cloud</span></span>

<span data-ttu-id="68ea0-133">Sie können auch eine vorhandene Cloud aktualisieren, sofern Sie über die erforderlichen Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="68ea0-134">Führen Sie diesen Schritt aus, wenn Sie zu einem anderen Azure-Profil wechseln oder einen Endpunkt hinzufügen oder ändern müssen.</span><span class="sxs-lookup"><span data-stu-id="68ea0-134">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="68ea0-135">Verwenden Sie dazu den Befehl `az cloud update`. Dieser akzeptiert die gleichen Argumente wie `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="68ea0-135">You do this with the `az cloud update` command, which takes the same arguments as `az cloud register`.</span></span> <span data-ttu-id="68ea0-136">Weitere Informationen finden Sie in der [Dokumentation für `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span><span class="sxs-lookup"><span data-stu-id="68ea0-136">For more information, see the [documentation for `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="68ea0-137">Aufheben der Registrierung einer Cloud</span><span class="sxs-lookup"><span data-stu-id="68ea0-137">Unregister a cloud</span></span>

<span data-ttu-id="68ea0-138">Wenn Sie eine registrierte Cloud nicht mehr benötigen, können Sie die Registrierung mit dem Befehl [cloud unregister](/cli/azure/cloud#unregister) aufheben:</span><span class="sxs-lookup"><span data-stu-id="68ea0-138">If you no longer require a registered cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```
