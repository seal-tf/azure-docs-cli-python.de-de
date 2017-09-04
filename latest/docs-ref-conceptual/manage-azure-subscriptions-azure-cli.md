---
title: Verwalten von Azure-Abonnements mit Azure CLI 2.0
description: Es wird beschrieben, wie Sie Azure-Abonnements mit Azure CLI 2.0 unter Linux, MacOS oder Windows verwalten.
keywords: Azure CLI 2.0, Linux, MacOS, Windows, OS X, Abonnement
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 383fb6ebd90ac79f60869187b402d53d4f1791fd
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2017
---
# <a name="manage-multiple-azure-subscriptions"></a>Verwalten mehrerer Azure-Abonnements

Falls Sie noch keine Erfahrung mit Azure haben, verfügen Sie wahrscheinlich nur über ein einzelnes Abonnement.
Falls Sie Azure hingegen schon eine Weile verwenden, haben Sie unter Umständen bereits mehrere Azure-Abonnements erstellt.
Wenn ja, können Sie Azure CLI 2.0 so konfigurieren, dass Befehle für ein bestimmtes Abonnement ausgeführt werden.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. Rufen Sie eine Liste mit allen Abonnements Ihres Kontos ab.

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

1. Legen Sie die Standardeinstellung fest.
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > Der `--subscription`-Parameter erhält den Namen des Abonnements oder die Abonnement-ID.

Sie können die Änderung überprüfen, indem Sie den Befehl `az account list --output table` erneut ausführen.

Nachdem Sie Ihr Standardabonnement festgelegt haben, werden alle weiteren Befehle der Azure-CLI für dieses Abonnement ausgeführt.