---
title: "Installieren der Azure-Befehlszeilenschnittstelle für Windows"
description: Installieren der Azure CLI 2.0 unter Windows
keywords: Azure CLI,Azure CLI installieren,Azure installieren Windows, Azure CLI Windows, Azure Windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="5b69f-104">Installieren der Azure CLI 2.0 unter Windows</span><span class="sxs-lookup"><span data-stu-id="5b69f-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="5b69f-105">Unter Windows können Sie über ein MSI-Installationsprogramm eine native Binärdatei installieren, die über die Windows-Eingabeaufforderung oder PowerShell verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="5b69f-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="5b69f-106">Wenn Sie das Windows-Subsystem für Linux (WSL) ausführen, sind Pakete für die ausgeführte Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5b69f-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="5b69f-107">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5b69f-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="5b69f-108">Installieren oder Aktualisieren mit MSI</span><span class="sxs-lookup"><span data-stu-id="5b69f-108">Install or update with MSI</span></span>

<span data-ttu-id="5b69f-109">Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="5b69f-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="5b69f-110">Sie können das [MSI-Installationsprogramm herunterladen](https://aka.ms/InstallAzureCliWindows) und anschließend zum Installieren oder Aktualisieren ausführen.</span><span class="sxs-lookup"><span data-stu-id="5b69f-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="5b69f-111">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="5b69f-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="5b69f-112">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="5b69f-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="5b69f-113">Deinstallieren mit der MSI-Datei</span><span class="sxs-lookup"><span data-stu-id="5b69f-113">Uninstall with MSI</span></span>

<span data-ttu-id="5b69f-114">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5b69f-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="5b69f-115">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="5b69f-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="5b69f-116">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="5b69f-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="5b69f-117">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5b69f-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="5b69f-118">Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5b69f-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="5b69f-119">Sie können das [MSI-Installationsprogramm herunterladen](https://aka.ms/InstallAzureCliWindows), wenn es nicht mehr auf Ihrem Computer verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="5b69f-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>
