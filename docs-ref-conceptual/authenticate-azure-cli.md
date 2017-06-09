---
title: Anmelden mit Azure CLI 2.0
description: Melden Sie sich mit Azure 2.0 CLI unter Linux, MacOS oder Windows an.
keywords: Azure CLI 2.0, Linux, MacOS, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2017
---
# <a name="log-in-with-azure-cli-20"></a>Anmelden mit Azure CLI 2.0

Es gibt mehrere Möglichkeiten, sich mit der Azure-CLI anzumelden und zu authentifizieren. Der einfachste erste Ansatz ist die interaktive Anmeldung per Browser oder über die Befehlszeile. Wir empfehlen die Verwendung von Dienstprinzipalen. Dies ermöglicht die Erstellung nicht interaktiver Konten für die Ressourcenbearbeitung. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

Befehle, die Sie mit der CLI ausführen, werden für Ihr Standardabonnement ausgeführt.  Wenn Sie über mehr als ein Abonnement verfügen, ist es ratsam, das [Standardabonnement zu bestätigen](manage-azure-subscriptions-azure-cli.md) und entsprechend zu ändern.

## <a name="interactive-log-in"></a>Interaktive Anmeldung

Melden Sie sich interaktiv über den Webbrowser an.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Befehlszeile

Geben Sie Ihre Anmeldeinformationen in der Befehlszeile an.

> [!Note]
> Dieser Ansatz funktioniert nicht für Microsoft-Konten oder Konten, für die die Authentifizierung in zwei Schritten aktiviert ist.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind vergleichbar mit Benutzerkonten, auf die Sie mithilfe von Azure Active Directory Regeln anwenden können.
Die Authentifizierung mit einem Dienstprinzipal ist die beste Möglichkeit, die Verwendung Ihrer Azure-Ressourcen mithilfe Ihrer Skripts oder Anwendungen zu schützen, mit denen Ressourcen bearbeitet werden.
Sie definieren die gewünschten Rollen für Ihre Benutzer mit dem Befehlssatz von `az role`.
Weitere Informationen und Beispiele für Dienstprinzipalrollen finden Sie unter den [Referenzartikeln zu „az role“](https://docs.microsoft.com/cli/azure/role.md).

1. Falls Sie noch nicht über einen Dienstprinzipal verfügen, [können Sie einen erstellen](create-an-azure-service-principal-azure-cli.md).

1. Melden Sie sich mit dem Dienstprinzipal an.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   Um Ihren Mandanten zu ermitteln, melden Sie sich interaktiv an und rufen anschließend die Mandanten-ID aus Ihrem Abonnement ab.

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```