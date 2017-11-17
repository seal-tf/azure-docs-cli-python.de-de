---
title: Verwalten mehrerer Clouds mit der Azure CLI 2.0
description: "Die Azure CLI 2.0 ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei verschiedenen Clouds."
keywords: Azure CLI 2.0, Azure, Clouds, Datencenter, Regierung, Region, China, Deutschland
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="5fac1-104">Verwalten mehrerer Clouds mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="5fac1-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="5fac1-105">Wenn mehrere Abonnements mit Azure verknüpft sind, stehen Ihnen unter Umständen mehrere Clouds zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="5fac1-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="5fac1-106">Jede Cloud verfügt über eigene zugeordnete Endpunkte und Funktionen und ist häufig einer bestimmten Region zugeordnet, für die unterschiedliche Datenschutzstandards oder -anforderungen gelten.</span><span class="sxs-lookup"><span data-stu-id="5fac1-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="5fac1-107">Für die effektive Verwendung mehrerer Clouds müssen Sie die derzeit aktive Cloud wechseln und ggf. neue Clouds erstellen können.</span><span class="sxs-lookup"><span data-stu-id="5fac1-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="5fac1-108">Auflisten von Clouds</span><span class="sxs-lookup"><span data-stu-id="5fac1-108">Listing clouds</span></span>

<span data-ttu-id="5fac1-109">Sie können die verfügbaren Clouds mit dem Befehl [cloud list](/cli/azure/cloud#list) auflisten.</span><span class="sxs-lookup"><span data-stu-id="5fac1-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="5fac1-110">Dadurch erfahren Sie, welche Cloud derzeit aktiv ist und wie das aktuelle Profil lautet. Darüber hinaus werden Informationen zu regionalen Suffixen und Hostnamen bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="5fac1-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="5fac1-111">So rufen Sie eine Liste der verfügbaren Clouds und die derzeit aktive Cloud ab:</span><span class="sxs-lookup"><span data-stu-id="5fac1-111">To get a list of the available clouds and the currently active one:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="5fac1-112">Wechseln der aktiven Cloud</span><span class="sxs-lookup"><span data-stu-id="5fac1-112">Switching the active cloud</span></span>

<span data-ttu-id="5fac1-113">Um die derzeit aktive Cloud zu wechseln, führen Sie den Befehl [cloud set](/cli/azure/cloud#set) aus.</span><span class="sxs-lookup"><span data-stu-id="5fac1-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="5fac1-114">Dieser Befehl erfordert ein Argument: den Namen der Cloud.</span><span class="sxs-lookup"><span data-stu-id="5fac1-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="5fac1-115">Wenn Sie sich nie für die aktive Cloud authentifiziert haben, müssen Sie dies vor dem Ausführen weiterer CLI-Vorgänge nachholen.</span><span class="sxs-lookup"><span data-stu-id="5fac1-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="5fac1-116">Anleitungen zur Authentifizierung finden Sie unter [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli) (Anmelden bei der Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="5fac1-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="5fac1-117">Registrieren oder Aufheben der Registrierung einer Cloud</span><span class="sxs-lookup"><span data-stu-id="5fac1-117">Register or unregister a cloud</span></span>

<span data-ttu-id="5fac1-118">Registrieren Sie eine neue Cloud, wenn Sie eigene Endpunkte besitzen oder ein anderes Profil benötigen.</span><span class="sxs-lookup"><span data-stu-id="5fac1-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="5fac1-119">Eine Cloud wird mit dem Befehl [cloud register](/cli/azure/cloud#register) erstellt.</span><span class="sxs-lookup"><span data-stu-id="5fac1-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="5fac1-120">Dieser Befehl erfordert einen Namen und optional einen Satz von Funktionen und Endpunktangaben.</span><span class="sxs-lookup"><span data-stu-id="5fac1-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="5fac1-121">So erstellen Sie eine Cloud mit einem spezialisierten Endpunkt für den Ressourcen-Manager und einem bestimmten Profil:</span><span class="sxs-lookup"><span data-stu-id="5fac1-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="5fac1-122">Dadurch wird die Cloud erstellt, aber _nicht_ automatisch ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="5fac1-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="5fac1-123">Wenn Sie die erstellte Cloud nicht mehr benötigen, kann ihre Registrierung mit dem Befehl [cloud unregister](/cli/azure/cloud#unregister) aufgehoben werden:</span><span class="sxs-lookup"><span data-stu-id="5fac1-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

