---
title: Anmelden mit Azure CLI 2.0
description: Melden Sie sich mit Azure 2.0 CLI unter Linux, MacOS oder Windows an.
keywords: Azure CLI 2.0, Anmeldung, Azure-Befehlszeilenschnittstelle, Azure CLI, Authentifizierung, autorisieren, anmelden
author: sptramer
ms.author: stttramer
manager: routlaw
ms.date: 11/13/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 0a8ec3541783ae19961f2acf1192c0ee061a465f
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2018
---
# <a name="log-in-with-azure-cli-20"></a>Anmelden mit Azure CLI 2.0

Es gibt mehrere Möglichkeiten, sich mit der Azure-CLI anzumelden und zu authentifizieren. Der einfachste erste Ansatz ist die interaktive Anmeldung per Browser oder über die Befehlszeile. Wir empfehlen die Verwendung von Dienstprinzipalen. Dies ermöglicht die Erstellung nicht interaktiver Konten für die Ressourcenbearbeitung. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

Die privaten Anmeldeinformationen werden nicht lokal gespeichert. Stattdessen wird von Azure ein Authentifizierungstoken generiert und gespeichert. Nach der Anmeldung ist das lokale Anmeldetoken gültig, bis es 14 Tage lang nicht verwendet wird. Dann müssen Sie sich erneut authentifizieren.

Nach der Anmeldung werden CLI-Befehle für Ihr Standardabonnement ausgeführt. Sollten Sie über mehrere Abonnements verfügen, empfiehlt es sich unter Umständen, das [Standardabonnement zu ändern](manage-azure-subscriptions-azure-cli.md).

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
Die Authentifizierung mit einem Dienstprinzipal ist die beste Möglichkeit, die Verwendung Ihrer Azure-Ressourcen mithilfe Ihrer Skripts oder Anwendungen zu schützen, mit denen Ressourcen bearbeitet werden. Falls Sie noch nicht über einen Dienstprinzipal verfügen und einen erstellen möchten, lesen Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0](create-an-azure-service-principal-azure-cli.md) weiter.

Für die Anmeldung mit einem Dienstprinzipal geben Sie den Benutzernamen, das Kennwort oder die PEM-Zertifikatdatei und den Mandanten an, der dem Dienstprinzipal zugeordnet ist:

```azurecli-interactive
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

Der Mandantenwert ist der dem Dienstprinzipal zugeordnete Azure Active Directory-Mandant. Hierbei kann es sich um eine Domäne vom Typ „onmicrosoft.com“ oder um die Azure-Objekt-ID für den Mandanten handeln.
Die Mandantenobjekt-ID für Ihre aktuelle Anmeldung können Sie mithilfe des folgenden Befehls abrufen:

```azurecli
az account show --query 'tenantId' -o tsv
```

