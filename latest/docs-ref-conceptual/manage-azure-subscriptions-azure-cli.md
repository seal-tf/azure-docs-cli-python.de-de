---
title: Verwalten von Azure-Abonnements mit Azure CLI 2.0
description: Es wird beschrieben, wie Sie Azure-Abonnements mit Azure CLI 2.0 unter Linux, MacOS oder Windows verwalten.
keywords: Azure CLI 2.0, Linux, MacOS, Windows, OS X, Abonnement
author: kamaljit
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: b4544d75aa279b5477f8497257d39182472fae71
ms.sourcegitcommit: 5db22de971cf3983785cb209d92cbed1bbd69ecf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/14/2017
---
# <a name="manage-multiple-azure-subscriptions"></a>Verwalten mehrerer Azure-Abonnements

Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement. Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure. Mehrere Abonnements lassen sich problemlos über die Befehlszeilenschnittstelle verwalten, und Vorgänge können durch Auswählen eines Abonnements ausgeführt werden.

## <a name="tenants-users-and-subscriptions"></a>Mandanten, Benutzer und Abonnements

Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren. Ein _Mandant_ ist ganz allgemein die Azure Active Directory-Entität, die eine gesamte Organisation umfasst. Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_. Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört. Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen bereitzustellen oder zu verwenden. Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln. Jede Ressource ist einem Abonnement zugeordnet.

Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).
Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/en-us/azure/active-directory/active-directory-how-subscriptions-associated-directory).

## <a name="working-with-multiple-subscriptions"></a>Verwenden mehrerer Abonnements

Für den Zugriff auf die Ressourcen in einem Abonnement müssen Sie Ihr aktives Abonnement wechseln. Alle Aufgaben im Zusammenhang mit Abonnements werden über den Befehl `az account` ausgeführt. Dieser verweist nicht auf Ihr individuelles Konto, sondern auf den Servicevertrag, den ein Abonnement darstellt.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

Wenn Sie mit Ihren verfügbaren Abonnements arbeiten möchten, rufen Sie zunächst eine Liste mit den verfügbaren Abonnements in Ihrem Konto ab:

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

Das aktive Abonnement können Sie mit `az account set` wechseln:

```azurecli-interactive
az account set --subscription "My Demos"
```

Verwenden Sie zum Auswählen des Abonnements entweder die Abonnement-ID oder den Namen des Abonnements.
