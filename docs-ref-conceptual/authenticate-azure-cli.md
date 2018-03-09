---
title: Anmelden mit Azure CLI 2.0
description: Melden Sie sich mit der Azure CLI 2.0 interaktiv oder mit lokalen Anmeldeinformationen an.
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 92c96b7e969de686689ef02bf068392b9f565698
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2018
---
# <a name="log-in-with-azure-cli-20"></a>Anmelden mit Azure CLI 2.0

Es gibt mehrere Möglichkeiten, sich mit der Azure-CLI anzumelden und zu authentifizieren. Melden Sie sich am besten interaktiv per Browser über Azure Cloud Shell oder den Befehl `az login` an.
Es wird empfohlen, Dienstprinzipale zu verwenden. Dabei handelt es sich um Konten mit eingeschränkten Berechtigungen. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

Die privaten Anmeldeinformationen werden nicht lokal gespeichert. Stattdessen wird von Azure ein Authentifizierungstoken generiert und gespeichert. Nach der Anmeldung ist das Anmeldetoken gültig, bis es 14 Tage lang nicht verwendet wird. Dann müssen Sie sich erneut authentifizieren.

Nach der Anmeldung werden CLI-Befehle für Ihr Standardabonnement ausgeführt. Sollten Sie über mehrere Abonnements verfügen, können Sie das [Standardabonnement ändern](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Interaktive Anmeldung

Melden Sie sich interaktiv über den Webbrowser an.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Befehlszeile

Geben Sie Ihre Anmeldeinformationen in der Befehlszeile an.

> [!Note]
> Dieser Ansatz funktioniert nicht für Microsoft-Konten oder Konten, für die die Authentifizierung in zwei Schritten aktiviert ist.

```azurecli
az login -u <username> -p <password>
```

## <a name="log-in-with-a-specific-tenant"></a>Anmelden mit einem bestimmten Mandanten

Wenn Sie mehrere Mandanten verwenden, können Sie mit dem Argument `--tenant` den Mandanten auswählen, unter dem Sie sich anmelden. Der Wert dieses Arguments kann eine Domäne vom Typ `.onmicrosoft.com` oder die Azure-Objekt-ID für den Mandanten sein. Sie können sich interaktiv anmelden oder Ihre Anmeldeinformationen mit den Argumenten `--user` und `--password` angeben. 

```
az login --tenant <tenant>
```

## <a name="logging-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind Konten, die nicht an einen bestimmten Benutzer gebunden sind und über Berechtigungen verfügen können, die ihnen über vordefinierte Rollen zugewiesen werden. Die Authentifizierung mit einem Dienstprinzipal ist die beste Methode zum Schreiben sicherer Skripts oder Programme und ermöglicht das Anwenden von Berechtigungseinschränkungen und lokal gespeicherten statischen Anmeldeinformationen. Weitere Informationen zu Dienstprinzipalen finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0](create-an-azure-service-principal-azure-cli.md).

Für die Anmeldung mit einem Dienstprinzipal geben Sie den Benutzernamen, das Kennwort oder die PEM-Zertifikatdatei und den Mandanten an, der dem Dienstprinzipal zugeordnet ist:

```azurecli
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

Der Mandantenwert ist der dem Dienstprinzipal zugeordnete Azure Active Directory-Mandant. Hierbei kann es sich um eine Domäne vom Typ `.onmicrosoft.com` oder um die Azure-Objekt-ID für den Mandanten handeln.
Die Mandantenobjekt-ID für Ihre aktuelle Anmeldung können Sie mithilfe des folgenden Befehls abrufen:

```azurecli
az account show --query 'tenantId' -o tsv
```
