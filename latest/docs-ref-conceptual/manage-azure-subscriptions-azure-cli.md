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
ms.openlocfilehash: c3538077e05d61f3c40880bb8b804226eb99dc85
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: de-DE
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="c7f66-104">Verwalten mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="c7f66-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="c7f66-105">Falls Sie noch keine Erfahrung mit Azure haben, verfügen Sie wahrscheinlich nur über ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c7f66-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="c7f66-106">Falls Sie Azure hingegen schon eine Weile verwenden, haben Sie unter Umständen bereits mehrere Azure-Abonnements erstellt.</span><span class="sxs-lookup"><span data-stu-id="c7f66-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="c7f66-107">Wenn ja, können Sie Azure CLI 2.0 so konfigurieren, dass Befehle für ein bestimmtes Abonnement ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="c7f66-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="c7f66-108">Rufen Sie eine Liste mit allen Abonnements Ihres Kontos ab.</span><span class="sxs-lookup"><span data-stu-id="c7f66-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="c7f66-109">Legen Sie die Standardeinstellung fest.</span><span class="sxs-lookup"><span data-stu-id="c7f66-109">Set the default.</span></span>
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

<span data-ttu-id="c7f66-110">Sie können die Änderung überprüfen, indem Sie den Befehl `az account list --output table` erneut ausführen.</span><span class="sxs-lookup"><span data-stu-id="c7f66-110">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="c7f66-111">Nachdem Sie Ihr Standardabonnement festgelegt haben, werden alle weiteren Befehle der Azure-CLI für dieses Abonnement ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="c7f66-111">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>