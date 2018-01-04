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
ms.openlocfilehash: 0f453ad1bff621250c8aa3147b5f5e916e712e30
ms.sourcegitcommit: 16426a08c0f2f62d0b9dca3df8132cece659acff
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/21/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="7ffcf-104">Verwalten mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="7ffcf-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="7ffcf-105">Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-105">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="7ffcf-106">Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-106">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="7ffcf-107">Mehrere Abonnements lassen sich problemlos über die Befehlszeilenschnittstelle verwalten, und Vorgänge können durch Auswählen eines Abonnements ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-107">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="7ffcf-108">Mandanten, Benutzer und Abonnements</span><span class="sxs-lookup"><span data-stu-id="7ffcf-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="7ffcf-109">Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="7ffcf-110">Ein _Mandant_ ist ganz allgemein die Azure Active Directory-Entität, die eine gesamte Organisation umfasst.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-110">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="7ffcf-111">Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="7ffcf-112">Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-112">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="7ffcf-113">Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen bereitzustellen oder zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-113">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="7ffcf-114">Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="7ffcf-115">Jede Ressource ist einem Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="7ffcf-116">Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="7ffcf-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="7ffcf-117">Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="7ffcf-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="7ffcf-118">Verwenden mehrerer Abonnements</span><span class="sxs-lookup"><span data-stu-id="7ffcf-118">Working with multiple subscriptions</span></span>

<span data-ttu-id="7ffcf-119">Für den Zugriff auf die Ressourcen in einem Abonnement müssen Sie Ihr aktives Abonnement wechseln.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-119">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="7ffcf-120">Alle Aufgaben im Zusammenhang mit Abonnements werden über den Befehl `az account` ausgeführt. Dieser verweist nicht auf Ihr individuelles Konto, sondern auf den Servicevertrag, den ein Abonnement darstellt.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-120">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="7ffcf-121">Wenn Sie mit Ihren verfügbaren Abonnements arbeiten möchten, rufen Sie zunächst eine Liste mit den verfügbaren Abonnements in Ihrem Konto ab:</span><span class="sxs-lookup"><span data-stu-id="7ffcf-121">To start working with your available subscriptions, get a list of those available in your account:</span></span>

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

<span data-ttu-id="7ffcf-122">Das aktive Abonnement können Sie mit `az account set` wechseln:</span><span class="sxs-lookup"><span data-stu-id="7ffcf-122">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="7ffcf-123">Verwenden Sie zum Auswählen des Abonnements entweder die Abonnement-ID oder den Namen des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-123">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
