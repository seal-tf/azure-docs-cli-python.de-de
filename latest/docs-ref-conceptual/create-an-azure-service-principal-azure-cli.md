---
title: Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0
description: "Hier erfahren Sie, wie Sie mit Azure CLI 2.0 einen Dienstprinzipal für Ihre App oder Ihren Dienst erstellen."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 10/12/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: a6ad5611f3e507b65e160122c87e22ec44546588
ms.sourcegitcommit: e8fe15e4f7725302939d726c75ba0fb3cad430be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0

Wenn Sie Ihre App oder Ihren Dienst mit Azure CLI 2.0 verwalten möchten, sollten Sie sie bzw. ihn nicht unter Ihren eigenen Anmeldeinformationen, sondern unter einem AAD-Dienstprinzipal (Azure Active Directory) ausführen.
In diesem Thema wird Schritt für Schritt erläutert, wie Sie einen Sicherheitsprinzipal mit Azure CLI 2.0 erstellen.

> [!NOTE]
> Dienstprinzipale können auch über das Azure-Portal erstellt werden.
> Ausführlichere Informationen finden Sie unter [Erstellen einer Active Directory-Anwendung und eines Dienstprinzipals mit Ressourcenzugriff mithilfe des Portals](/azure/azure-resource-manager/resource-group-create-service-principal-portal).

## <a name="what-is-a-service-principal"></a>Was ist ein Dienstprinzipal?

Ein Azure-Dienstprinzipal ist eine Sicherheitsidentität, die durch von Benutzern erstellte Apps, Dienste und Automatisierungstools verwendet wird, um auf bestimmte Azure-Ressourcen zuzugreifen. Das Konzept lässt sich als Benutzeridentität (Anmeldename und Kennwort oder Zertifikat) mit einer bestimmten Rolle und streng kontrollierten Berechtigungen für den Ressourcenzugriff beschreiben. Im Gegensatz zu einer allgemeinen Benutzeridentität muss diese Identität nur ganz bestimmte Aktionen ausführen können. Wenn Sie ihr nur die Berechtigungen gewähren, die sie zum Ausführen ihrer Verwaltungsaufgaben benötigt, verbessert das die Sicherheit. 

Azure CLI 2.0 unterstützt die Erstellung von kennwortbasierten Anmeldeinformationen für die Authentifizierung und von Zertifikatanmeldeinformationen. In diesem Thema werden beide Arten von Anmeldeinformationen behandelt.

## <a name="verify-your-own-permission-level"></a>Überprüfen der eigenen Berechtigungsstufe

Zunächst einmal müssen Sie sowohl in der Azure Active Directory-Instanz als auch im Azure-Abonnement über ausreichende Berechtigungen verfügen. Sie müssen insbesondere eine App in der Active Directory-Instanz erstellen und dem Dienstprinzipal eine Rolle zuweisen können. 

Die einfachste Möglichkeit zum Überprüfen, ob Ihr Konto über die erforderlichen Berechtigungen verfügt, ist über das Portal. Siehe [Überprüfen der erforderlichen Berechtigung im Portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).

## <a name="create-a-service-principal-for-your-application"></a>Erstellen eines Dienstprinzipals für Ihre Anwendung

Sie müssen über eine der folgenden Angaben verfügen, um die App identifizieren zu können, für die Sie einen Dienstprinzipal erstellen möchten:

  * Eindeutigen Namen oder URI Ihrer bereitgestellten App („MyDemoWebApp“ in den folgenden Beispielen)
  * Anwendungs-ID (GUID, die Ihrer bereitgestellten App, Ihrem bereitgestellten Dienst oder Ihrem bereitgestellten Objekt zugeordnet ist)

Mit diesen Werten wird Ihre Anwendung bei der Erstellung eines Dienstprinzipals identifiziert.

### <a name="get-information-about-your-application"></a>Abrufen von Informationen zu Ihrer Anwendung

Rufen Sie Identitätsinformationen zu Ihrer Anwendung mithilfe von `az ad app list` ab.

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

Mit der Option `--display-name` wird die zurückgegebene Liste mit den Apps gefiltert, um nur die Apps anzuzeigen, für die `displayName` mit „MyDemoWebApp“ beginnt.

### <a name="create-a-service-principal-with-a-password"></a>Erstellen eines Dienstprinzipals mit einem Kennwort

Verwenden Sie [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) und den Parameter `--password`, um den Dienstprinzipal mit einem Kennwort zu erstellen. Wenn Sie keine Rolle bzw. keinen Bereich angeben, wird für das aktuelle Abonnement standardmäßig die Rolle **Mitwirkender** festgelegt. Wenn Sie für die Erstellung des Dienstprinzipals weder den Parameter `--password` noch den Parameter `--cert` verwenden, wird die Kennwortauthentifizierung verwendet, und ein Kennwort wird für Sie erstellt.

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
 > Vermeiden Sie es, ein unsicheres Kennwort zu erstellen.  Befolgen Sie die Anleitung unter [Kennwortrichtlinien und -einschränkungen in Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).

### <a name="create-a-service-principal-with-a-self-signed-certificate"></a>Erstellen eines Dienstprinzipals mit einem selbstsignierten Zertifikat

Verwenden Sie [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) und den Parameter `--create-cert`, um ein selbstsigniertes Zertifikat zu erstellen.

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --create-cert
```

```json
{
  "appId": "c495db57-82e0-4e2e-9369-069dff176858",
  "displayName": "azure-cli-2017-10-12-22-15-38",
  "fileWithCertAndPrivateKey": "<path>/<file-name>.pem",
  "name": "http://MyDemoWebApp",
  "password": null,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Kopieren Sie den Wert der `fileWithCertAndPrivateKey`-Antwort. Hierbei handelt es sich um die für die Authentifizierung verwendete Zertifikatdatei.

Weitere Optionen für die Verwendung von Zertifikaten finden Sie unter [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).

### <a name="get-information-about-the-service-principal"></a>Abrufen von Informationen zum Dienstprinzipal

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

### <a name="sign-in-using-the-service-principal"></a>Anmelden mithilfe des Dienstprinzipals

Sie können sich nun als neuer Dienstprinzipal für Ihre App anmelden. Verwenden Sie dazu *appId* aus `az ad sp show` und entweder das *Kennwort* oder den Pfad zum erstellten Zertifikat.  Geben Sie den Wert für *tenant* aus den Ergebnissen von `az ad sp create-for-rbac` an.

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password-or-path-to-cert} --tenant {tenant}
``` 

Nach einer erfolgreichen Anmeldung wird diese Ausgabe angezeigt:

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

Verwenden Sie die Werte `id`, `password` und `tenant` als Anmeldeinformationen zum Ausführen Ihrer App. 

## <a name="managing-roles"></a>Verwalten von Rollen 

> [!NOTE]
> Bei der rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) in Azure handelt es sich um ein Modell zum Definieren und Verwalten von Rollen für Benutzer- und Dienstprinzipale.
> Rollen sind bestimmte Berechtigungen zugeordnet, die bestimmen, welche Ressourcen ein Prinzipal lesen, aufrufen, schreiben oder verwalten kann.
> Weitere Informationen zu RBAC und Rollen finden Sie unter [Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).

Azure CLI 2.0 enthält die folgenden Befehle zum Verwalten von Rollenzuweisungen:

* [az role assignment list](/cli/azure/role/assignment#list)
* [az role assignment create](/cli/azure/role/assignment#create)
* [az role assignment delete](/cli/azure/role/assignment#delete)

Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**. Dies ist unter Umständen nicht die beste Wahl für die Interaktionen einer App, da diese Rolle über umfassende Berechtigungen verfügt. Die Rolle **Leser** ist stärker eingeschränkt und ist eine gute Wahl für den schreibgeschützten Zugriff. Über das Azure-Portal können Sie Details zu rollenspezifischen Berechtigungen anzeigen oder benutzerdefinierte Berechtigungen erstellen.

Im folgenden Beispiel wird dem vorherigen Beispiel die Rolle **Leser** hinzugefügt und die Rolle **Mitwirkender** gelöscht:

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

Überprüfen Sie die Änderungen, indem Sie die derzeit zugewiesenen Rollen auflisten:

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
> Wenn Ihr Konto nicht über ausreichende Berechtigungen zum Zuweisen einer Rolle verfügt, wird eine Fehlermeldung angezeigt.
> In der Meldung ist angegeben, dass Ihr Konto keine Berechtigung zum Ausführen der Aktion „Microsoft.Authorization/roleAssignments/write“ über Bereich „/subscriptions/{guid}“ hat.
   
## <a name="change-the-credentials-of-a-security-principal"></a>Ändern der Anmeldeinformationen eines Sicherheitsprinzipals

Aus Sicherheitsgründen empfiehlt es sich, regelmäßig die Berechtigungen zu überprüfen und die Kennwörter zu aktualisieren. Darüber hinaus sollten Sie auch die Sicherheitsanmeldeinformationen verwalten und ändern, wenn sich Ihre App verändert.

### <a name="reset-a-service-principal-password"></a>Zurücksetzen des Kennworts eines Dienstprinzipals

Verwenden Sie `az ad sp reset-credentials`, um das aktuelle Kennwort für den Dienstprinzipal zurückzusetzen.

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

Die CLI generiert ein sicheres Kennwort, wenn Sie die Option `--password` weglassen.
