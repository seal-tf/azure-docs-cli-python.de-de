---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI 2.0 unter Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 27284520d923524c5f772c82246889b2f1e6cb8b
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="22187-103">Installieren der Azure CLI 2.0 unter Windows</span><span class="sxs-lookup"><span data-stu-id="22187-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="22187-104">Unter Windows wird die Binärdatei der Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.</span><span class="sxs-lookup"><span data-stu-id="22187-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="22187-105">Bei Verwendung des Windows-Subsystems für Linux (WSL) sind Pakete für Ihre Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="22187-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="22187-106">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="22187-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="22187-107">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="22187-107">Install or update</span></span>

<span data-ttu-id="22187-108">Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="22187-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="22187-109">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="22187-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="22187-110">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="22187-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="22187-111">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="22187-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="22187-112">In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="22187-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="22187-113">Führen Sie den Befehl `az login` aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="22187-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="22187-114">Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="22187-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="22187-115">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="22187-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="22187-116">Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="22187-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="22187-117">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="22187-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
