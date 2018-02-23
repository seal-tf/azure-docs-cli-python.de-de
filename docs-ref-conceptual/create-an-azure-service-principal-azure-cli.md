---
title: Verwenden von Azure-Dienstprinzipalen mit der Azure CLI 2.0
description: Hier erfahren Sie, wie Sie mit der Azure CLI 2.0 einen Dienstprinzipal erstellen und verwenden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/12/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b46c735a14240bddd07659475ada1c33c75a1e67
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="e47a7-103">Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e47a7-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="e47a7-104">Wenn Sie eine separate Anmeldung mit Zugriffseinschränkungen erstellen möchten, können Sie dafür einen Dienstprinzipal verwenden.</span><span class="sxs-lookup"><span data-stu-id="e47a7-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="e47a7-105">Dienstprinzipale sind separate Identitäten, die einem Konto zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="e47a7-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="e47a7-106">Dienstprinzipale sind hilfreich bei der Verwendung von Anwendungen und Tasks, die automatisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="e47a7-107">Dieser Artikel führt Sie durch den Vorgang zum Erstellen eines Dienstprinzipals.</span><span class="sxs-lookup"><span data-stu-id="e47a7-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="e47a7-108">Erstellen des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="e47a7-108">Create the service principal</span></span>

<span data-ttu-id="e47a7-109">Verwenden Sie den Befehl [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac), um einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="e47a7-110">Der Name des Dienstprinzipals ist nicht mit dem vorhandenen Namen einer Anwendung oder eines Benutzers verknüpft.</span><span class="sxs-lookup"><span data-stu-id="e47a7-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="e47a7-111">Sie können einen Dienstprinzipal mit dem gewünschten Authentifizierungstyp erstellen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="e47a7-112">`--password` wird für die kennwortbasierte Authentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="e47a7-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="e47a7-113">Halten Sie sich an die Vorgaben unter [Kennwortrichtlinien und -einschränkungen in Azure Active Directory](/azure/active-directory/active-directory-passwords-policy), um ein sicheres Kennwort zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="e47a7-114">Falls Sie kein Kennwort angeben, wird eines für Sie erstellt.</span><span class="sxs-lookup"><span data-stu-id="e47a7-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="e47a7-115">`--cert` wird für die zertifikatbasierte Authentifizierung für ein vorhandenes Zertifikat verwendet (entweder als öffentliche PEM- oder DER-Zeichenfolge oder als `@{file}` zum Laden einer Datei).</span><span class="sxs-lookup"><span data-stu-id="e47a7-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="e47a7-116">Das Argument `--keyvault` kann hinzugefügt werden, um anzugeben, dass das Zertifikat in Azure Key Vault gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="e47a7-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="e47a7-117">In diesem Fall verweist der Wert `--cert` auf den Namen des Zertifikats in Key Vault.</span><span class="sxs-lookup"><span data-stu-id="e47a7-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

* <span data-ttu-id="e47a7-118">`--create-cert` erstellt ein _selbstsigniertes_ Zertifikat für die Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="e47a7-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="e47a7-119">Das Argument `--keyvault` kann hinzugefügt werden, um das Zertifikat in Azure Key Vault zu speichern.</span><span class="sxs-lookup"><span data-stu-id="e47a7-119">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

<span data-ttu-id="e47a7-120">Wenn kein Argument angegeben wird, das den Authentifizierungstyp angibt, wird standardmäßig `--password` verwendet.</span><span class="sxs-lookup"><span data-stu-id="e47a7-120">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="e47a7-121">Die Ausgabe des Befehls `create-for-rbac` hat folgendes Format:</span><span class="sxs-lookup"><span data-stu-id="e47a7-121">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="e47a7-122">Die Werte `appId`, `tenant` und `password` werden für die Authentifizierung verwendet.</span><span class="sxs-lookup"><span data-stu-id="e47a7-122">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="e47a7-123">`displayName` wird bei der Suche nach einem vorhandenen Dienstprinzipal verwendet.</span><span class="sxs-lookup"><span data-stu-id="e47a7-123">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="e47a7-124">Wenn Ihr Konto nicht über ausreichende Berechtigungen zum Erstellen eines Dienstprinzipals verfügt, wird eine Fehlermeldung mit dem Hinweis „Nicht genügend Berechtigungen zum Abschließen des Vorgangs“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e47a7-124">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="e47a7-125">Bitten Sie den Azure Active Directory-Administrator, einen Dienstprinzipal zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-125">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="e47a7-126">Verwalten von Dienstprinzipalrollen</span><span class="sxs-lookup"><span data-stu-id="e47a7-126">Manage service principal roles</span></span> 

<span data-ttu-id="e47a7-127">Die Azure CLI 2.0 enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:</span><span class="sxs-lookup"><span data-stu-id="e47a7-127">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="e47a7-128">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="e47a7-128">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="e47a7-129">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="e47a7-129">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="e47a7-130">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="e47a7-130">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="e47a7-131">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="e47a7-131">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="e47a7-132">Diese Rolle besitzt uneingeschränkte Berechtigungen für Lese- und Schreibvorgänge in einem Azure-Konto. Sie eignet sich in der Regel nicht für Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-132">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="e47a7-133">Die Rolle **Leser** ist stärker eingeschränkt und bietet schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="e47a7-133">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="e47a7-134">Weitere Informationen zur rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) und zu Rollen finden Sie unter [Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="e47a7-134">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="e47a7-135">Dieses Beispiel fügt die Rolle **Leser** hinzu und löscht die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="e47a7-135">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="e47a7-136">Durch das Hinzufügen einer Rolle werden zuvor zugewiesene Berechtigungen _nicht_ geändert.</span><span class="sxs-lookup"><span data-stu-id="e47a7-136">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="e47a7-137">Beim Einschränken der Berechtigungen eines Dienstprinzipals sollte immer die Rolle __Mitwirkender__ entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="e47a7-137">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="e47a7-138">Die Änderungen können durch Auflisten der zugewiesenen Rollen überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="e47a7-138">The changes can be verified by listing the assigned roles.</span></span>

```azurecli
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="e47a7-139">Wenn Ihr Konto nicht über die Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ über Bereich „/subscriptions/{guid}“ hat. Bitten Sie den Azure Active Directory-Administrator um die Verwaltung von Rollen.</span><span class="sxs-lookup"><span data-stu-id="e47a7-139">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="log-in-using-the-service-principal"></a><span data-ttu-id="e47a7-140">Anmelden mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="e47a7-140">Log in using the service principal</span></span>

<span data-ttu-id="e47a7-141">Sie können die Anmeldung und Berechtigungen des neuen Dienstprinzipals testen, indem Sie sich darunter bei der Azure CLI anmelden.</span><span class="sxs-lookup"><span data-stu-id="e47a7-141">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="e47a7-142">Melden Sie sich mit den Werten für `appId`, `tenant` und die Anmeldeinformationen an.</span><span class="sxs-lookup"><span data-stu-id="e47a7-142">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="e47a7-143">Die von Ihnen angegebenen Authentifizierungsinformationen ändern sich basierend darauf, ob Sie den Dienstprinzipal mit einem Kennwort oder mit einem Zertifikat erstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="e47a7-143">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="e47a7-144">Wenn Sie sich mit einem Kennwort anmelden möchten, geben Sie es als Argumentparameter an.</span><span class="sxs-lookup"><span data-stu-id="e47a7-144">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="e47a7-145">Um sich mit einem Zertifikat anmelden zu können, muss es lokal als PEM- oder DER-Datei verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="e47a7-145">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```
## <a name="reset-credentials"></a><span data-ttu-id="e47a7-146">Zurücksetzen von Anmeldeinformation</span><span class="sxs-lookup"><span data-stu-id="e47a7-146">Reset credentials</span></span>

<span data-ttu-id="e47a7-147">Falls Sie die Anmeldeinformationen für einen Dienstprinzipal vergessen, können sie mit dem Befehl [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials) zurückgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="e47a7-147">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials) command.</span></span> <span data-ttu-id="e47a7-148">Hier gelten die gleichen Einschränkungen und Optionen wie beim Erstellen eines neuen Dienstprinzipals.</span><span class="sxs-lookup"><span data-stu-id="e47a7-148">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
