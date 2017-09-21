---
title: Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0
description: "Hier erfahren Sie, wie Sie mit Azure CLI 2.0 einen Dienstprinzipal für Ihre App oder Ihren Dienst erstellen."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: 0ee794d5a732c6e8d2d52fca5810a874827930ae
ms.sourcegitcommit: 5a04b7fbb73a5f10c4021963ecd6ebe234cc3b61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/15/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="99a63-104">Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="99a63-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="99a63-105">Wenn Sie Ihre App oder Ihren Dienst mit Azure CLI 2.0 verwalten möchten, sollten Sie sie bzw. ihn nicht unter Ihren eigenen Anmeldeinformationen, sondern unter einem AAD-Dienstprinzipal (Azure Active Directory) ausführen.</span><span class="sxs-lookup"><span data-stu-id="99a63-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="99a63-106">In diesem Thema wird Schritt für Schritt erläutert, wie Sie einen Sicherheitsprinzipal mit Azure CLI 2.0 erstellen.</span><span class="sxs-lookup"><span data-stu-id="99a63-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="99a63-107">Dienstprinzipale können auch über das Azure-Portal erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="99a63-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="99a63-108">Ausführlichere Informationen finden Sie unter [Erstellen einer Active Directory-Anwendung und eines Dienstprinzipals mit Ressourcenzugriff mithilfe des Portals](/azure/azure-resource-manager/resource-group-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="99a63-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="99a63-109">Was ist ein Dienstprinzipal?</span><span class="sxs-lookup"><span data-stu-id="99a63-109">What is a 'service principal'?</span></span>

<span data-ttu-id="99a63-110">Ein Azure-Dienstprinzipal ist eine Sicherheitsidentität, die durch von Benutzern erstellte Apps, Dienste und Automatisierungstools verwendet wird, um auf bestimmte Azure-Ressourcen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="99a63-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="99a63-111">Das Konzept lässt sich als Benutzeridentität (Anmeldename und Kennwort oder Zertifikat) mit einer bestimmten Rolle und streng kontrollierten Berechtigungen für den Ressourcenzugriff beschreiben.</span><span class="sxs-lookup"><span data-stu-id="99a63-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="99a63-112">Im Gegensatz zu einer allgemeinen Benutzeridentität muss diese Identität nur ganz bestimmte Aktionen ausführen können.</span><span class="sxs-lookup"><span data-stu-id="99a63-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="99a63-113">Wenn Sie ihr nur die Berechtigungen gewähren, die sie zum Ausführen ihrer Verwaltungsaufgaben benötigt, verbessert das die Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="99a63-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="99a63-114">Derzeit unterstützt Azure CLI 2.0 nur die Erstellung von kennwortbasierten Anmeldeinformationen für die Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="99a63-114">Right now, Azure CLI 2.0 only supports the creation of password-based authentication credentials.</span></span> <span data-ttu-id="99a63-115">In diesem Thema werden das Erstellen eines Dienstprinzipals mit einem bestimmten Kennwort und das optionale Zuweisen von bestimmten Rollen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="99a63-115">In this topic, we cover creating a service principal with a specific password, and optionally assigning specific roles to it.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="99a63-116">Überprüfen der eigenen Berechtigungsstufe</span><span class="sxs-lookup"><span data-stu-id="99a63-116">Verify your own permission level</span></span>

<span data-ttu-id="99a63-117">Zunächst einmal müssen Sie sowohl in der Azure Active Directory-Instanz als auch im Azure-Abonnement über ausreichende Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="99a63-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="99a63-118">Sie müssen insbesondere eine App in der Active Directory-Instanz erstellen und dem Dienstprinzipal eine Rolle zuweisen können.</span><span class="sxs-lookup"><span data-stu-id="99a63-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="99a63-119">Die einfachste Möglichkeit zum Überprüfen, ob Ihr Konto über die erforderlichen Berechtigungen verfügt, ist über das Portal.</span><span class="sxs-lookup"><span data-stu-id="99a63-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="99a63-120">Siehe [Überprüfen der erforderlichen Berechtigung im Portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="99a63-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="99a63-121">Erstellen eines Dienstprinzipals für Ihre Anwendung</span><span class="sxs-lookup"><span data-stu-id="99a63-121">Create a service principal for your application</span></span>

<span data-ttu-id="99a63-122">Sie müssen über eine der folgenden Angaben verfügen, um die App identifizieren zu können, für die Sie einen Dienstprinzipal erstellen möchten:</span><span class="sxs-lookup"><span data-stu-id="99a63-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="99a63-123">Eindeutigen Namen oder URI Ihrer bereitgestellten App („MyDemoWebApp“ in den folgenden Beispielen)</span><span class="sxs-lookup"><span data-stu-id="99a63-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="99a63-124">Anwendungs-ID (GUID, die Ihrer bereitgestellten App, Ihrem bereitgestellten Dienst oder Ihrem bereitgestellten Objekt zugeordnet ist)</span><span class="sxs-lookup"><span data-stu-id="99a63-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="99a63-125">Mit diesen Werten wird Ihre Anwendung bei der Erstellung eines Dienstprinzipals identifiziert.</span><span class="sxs-lookup"><span data-stu-id="99a63-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="99a63-126">Abrufen von Informationen zu Ihrer Anwendung</span><span class="sxs-lookup"><span data-stu-id="99a63-126">Get information about your application</span></span>

<span data-ttu-id="99a63-127">Rufen Sie Identitätsinformationen zu Ihrer Anwendung mithilfe von `az ad app list` ab.</span><span class="sxs-lookup"><span data-stu-id="99a63-127">Get identity information about your application with the `az ad app list`.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

<span data-ttu-id="99a63-128">Mit der Option `--display-name` wird die zurückgegebene Liste mit den Apps gefiltert, um nur die Apps anzuzeigen, für die `displayName` mit „MyDemoWebApp“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="99a63-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-the-service-principal"></a><span data-ttu-id="99a63-129">Erstellen des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="99a63-129">Create the service principal</span></span>

<span data-ttu-id="99a63-130">Verwenden Sie [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac), um den Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="99a63-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) to create the service principal.</span></span> 

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
``` 

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING] 
 > <span data-ttu-id="99a63-131">Vermeiden Sie es, ein unsicheres Kennwort zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="99a63-131">Don't create an insecure password.</span></span>  <span data-ttu-id="99a63-132">Befolgen Sie die Anleitung unter [Kennwortrichtlinien und -einschränkungen in Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="99a63-132">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="99a63-133">Abrufen von Informationen zum Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="99a63-133">Get information about the service principal</span></span>

```azurecli-interactive
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="99a63-134">Anmelden mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="99a63-134">Sign in using the service principal</span></span>

<span data-ttu-id="99a63-135">Nun können Sie sich als der neue Dienstprinzipal für die App anmelden. Verwenden Sie hierbei die Werte für *appId* und *password* aus `az ad sp show`.</span><span class="sxs-lookup"><span data-stu-id="99a63-135">You can now log in as the new service principal for your app using the *appId* and *password* from `az ad sp show`.</span></span>  <span data-ttu-id="99a63-136">Geben Sie den Wert für *tenant* aus den Ergebnissen von `az ad sp create-for-rbac` an.</span><span class="sxs-lookup"><span data-stu-id="99a63-136">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

<span data-ttu-id="99a63-137">Nach einer erfolgreichen Anmeldung wird diese Ausgabe angezeigt:</span><span class="sxs-lookup"><span data-stu-id="99a63-137">You will see this output after a successful sign-on:</span></span>

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

<span data-ttu-id="99a63-138">Verwenden Sie die Werte `id`, `password` und `tenant` als Anmeldeinformationen zum Ausführen Ihrer App.</span><span class="sxs-lookup"><span data-stu-id="99a63-138">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="99a63-139">Verwalten von Rollen</span><span class="sxs-lookup"><span data-stu-id="99a63-139">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="99a63-140">Bei der rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) in Azure handelt es sich um ein Modell zum Definieren und Verwalten von Rollen für Benutzer- und Dienstprinzipale.</span><span class="sxs-lookup"><span data-stu-id="99a63-140">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="99a63-141">Rollen sind bestimmte Berechtigungen zugeordnet, die bestimmen, welche Ressourcen ein Prinzipal lesen, aufrufen, schreiben oder verwalten kann.</span><span class="sxs-lookup"><span data-stu-id="99a63-141">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="99a63-142">Weitere Informationen zu RBAC und Rollen finden Sie unter [Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="99a63-142">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="99a63-143">Azure CLI 2.0 enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:</span><span class="sxs-lookup"><span data-stu-id="99a63-143">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="99a63-144">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="99a63-144">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="99a63-145">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="99a63-145">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="99a63-146">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="99a63-146">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="99a63-147">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="99a63-147">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="99a63-148">Dies ist unter Umständen nicht die beste Wahl für die Interaktionen einer App, da diese Rolle über umfassende Berechtigungen verfügt.</span><span class="sxs-lookup"><span data-stu-id="99a63-148">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="99a63-149">Die Rolle **Leser** ist stärker eingeschränkt und ist eine gute Wahl für den schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="99a63-149">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="99a63-150">Über das Azure-Portal können Sie Details zu rollenspezifischen Berechtigungen anzeigen oder benutzerdefinierte Berechtigungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="99a63-150">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="99a63-151">Im folgenden Beispiel wird dem vorherigen Beispiel die Rolle **Leser** hinzugefügt und die Rolle **Mitwirkender** gelöscht:</span><span class="sxs-lookup"><span data-stu-id="99a63-151">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="99a63-152">Überprüfen Sie die Änderungen, indem Sie die derzeit zugewiesenen Rollen auflisten:</span><span class="sxs-lookup"><span data-stu-id="99a63-152">Verify the changes by listing the currently assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE] 
> <span data-ttu-id="99a63-153">Wenn Ihr Konto nicht über ausreichende Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="99a63-153">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="99a63-154">In der Meldung ist angegeben, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ über Bereich „/subscriptions/{guid}“ hat.</span><span class="sxs-lookup"><span data-stu-id="99a63-154">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="99a63-155">Ändern der Anmeldeinformationen eines Sicherheitsprinzipals</span><span class="sxs-lookup"><span data-stu-id="99a63-155">Change the credentials of a security principal</span></span>

<span data-ttu-id="99a63-156">Aus Sicherheitsgründen empfiehlt es sich, regelmäßig die Berechtigungen zu überprüfen und die Kennwörter zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="99a63-156">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="99a63-157">Darüber hinaus sollten Sie auch die Sicherheitsanmeldeinformationen verwalten und ändern, wenn sich Ihre App verändert.</span><span class="sxs-lookup"><span data-stu-id="99a63-157">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="99a63-158">Zurücksetzen des Kennworts eines Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="99a63-158">Reset a service principal password</span></span>

<span data-ttu-id="99a63-159">Verwenden Sie `az ad sp reset-credentials`, um das aktuelle Kennwort für den Dienstprinzipal zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="99a63-159">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

```azurecli-interactive
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="99a63-160">Die CLI generiert ein sicheres Kennwort, wenn Sie die Option `--password` weglassen.</span><span class="sxs-lookup"><span data-stu-id="99a63-160">The CLI generates a secure password if you leave out the `--password` option.</span></span>