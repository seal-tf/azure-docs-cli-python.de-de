---
title: "Installieren der Azure-Befehlszeilenschnittstelle für Windows"
description: Installieren der Azure CLI 2.0 unter Windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3e732ea7fae118ddb1564bed28d54d15bab4f7f0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="2af59-103">Installieren der Azure CLI 2.0 unter Windows</span><span class="sxs-lookup"><span data-stu-id="2af59-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="2af59-104">Unter Windows wird die Binärdatei der Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.</span><span class="sxs-lookup"><span data-stu-id="2af59-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="2af59-105">Bei Verwendung des Windows-Subsystems für Linux (WSL) sind Pakete für Ihre Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2af59-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="2af59-106">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2af59-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="2af59-107">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2af59-107">Install or update</span></span>

<span data-ttu-id="2af59-108">Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="2af59-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="2af59-109">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="2af59-109">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

<span data-ttu-id="2af59-110">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="2af59-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="2af59-111">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="2af59-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="2af59-112">In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Eingabeaufforderung nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="2af59-112">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="2af59-113">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="2af59-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="2af59-114">Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="2af59-114">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="2af59-115">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="2af59-115">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
