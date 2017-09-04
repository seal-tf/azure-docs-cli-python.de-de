---
title: Azure CLI 2.0
description: "Enthält eine Übersicht über Azure CLI 2.0."
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
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: de-DE
---
# <a name="azure-cli-20"></a><span data-ttu-id="a5c3c-104">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a5c3c-104">Azure CLI 2.0</span></span>

<span data-ttu-id="a5c3c-105">Azure CLI 2.0 ist die neue Befehlszeilenumgebung von Azure und dient zum Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>  <span data-ttu-id="a5c3c-106">Sie kann unter MacOS, Linux und Windows verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-106">It can be used on macOS, Linux, and Windows.</span></span> 

<span data-ttu-id="a5c3c-107">Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="a5c3c-108">Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:</span><span class="sxs-lookup"><span data-stu-id="a5c3c-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="a5c3c-109">In [diesem Artikel](install-azure-cli.md) erfahren Sie, wie Sie Azure CLI 2.0 auf Ihrem System installieren und einrichten.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-109">Review the [Install article](install-azure-cli.md) to get Azure CLI 2.0 up and running on your system.</span></span> <span data-ttu-id="a5c3c-110">Lesen Sie anschließend den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mit der Verwendung zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-110">Then read the [Get Started](get-started-with-azure-cli.md) article to begin using it.</span></span>
<span data-ttu-id="a5c3c-111">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a5c3c-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="a5c3c-112">In den folgenden Beispielen werden gängige Szenarien mit Azure CLI 2.0 veranschaulicht:</span><span class="sxs-lookup"><span data-stu-id="a5c3c-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="a5c3c-113">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="a5c3c-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="a5c3c-114">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="a5c3c-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="a5c3c-115">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="a5c3c-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="a5c3c-116">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="a5c3c-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="a5c3c-117">Außerdem ist eine ausführliche [Referenz](/cli/azure/) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="a5c3c-118">Führen Sie jetzt die [ersten Schritte](get-started-with-azure-cli.md) mit Azure CLI 2.0 aus.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="a5c3c-119">Falls Sie die vorherige Version der CLI (Azure-CLI) nutzen, können Sie sie weiterverwenden.</span><span class="sxs-lookup"><span data-stu-id="a5c3c-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="a5c3c-120">Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="a5c3c-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 