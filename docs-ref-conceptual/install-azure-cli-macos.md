---
title: "Installieren der Azure-Befehlszeilenschnittstelle für macOS"
description: Installieren der Azure CLI 2.0 unter macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0295846abc2fe6091940824c6efc47b8fd64ce9f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="6fe93-103">Installieren der Azure CLI 2.0 unter macOS</span><span class="sxs-lookup"><span data-stu-id="6fe93-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="6fe93-104">Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](http://brew.sh) installieren.</span><span class="sxs-lookup"><span data-stu-id="6fe93-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="6fe93-105">Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten.</span><span class="sxs-lookup"><span data-stu-id="6fe93-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="6fe93-106">Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.</span><span class="sxs-lookup"><span data-stu-id="6fe93-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="6fe93-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="6fe93-107">Install</span></span>

<span data-ttu-id="6fe93-108">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="6fe93-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="6fe93-109">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="6fe93-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="6fe93-110">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="6fe93-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="6fe93-111">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="6fe93-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="6fe93-112">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="6fe93-112">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6fe93-113">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="6fe93-113">Troubleshooting</span></span>

<span data-ttu-id="6fe93-114">In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können.</span><span class="sxs-lookup"><span data-stu-id="6fe93-114">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="6fe93-115">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6fe93-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="6fe93-116">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="6fe93-116">Unable to find Python or installed packages</span></span>

<span data-ttu-id="6fe93-117">Sollten Python oder installierte Pakete bei der Installation nicht gefunden werden, weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor, das während der Homebrew-Installation aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="6fe93-117">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="6fe93-118">Da die CLI keine virtuelle Python-Umgebung verwendet, muss sie die korrekte Python-Version finden können.</span><span class="sxs-lookup"><span data-stu-id="6fe93-118">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="6fe93-119">Zur Behebung dieser Probleme können Sie ggf. die Python-Installation neu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="6fe93-119">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="6fe93-120">CLI-Version 1.x wird installiert.</span><span class="sxs-lookup"><span data-stu-id="6fe93-120">CLI version 1.x is installed</span></span>

<span data-ttu-id="6fe93-121">Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein.</span><span class="sxs-lookup"><span data-stu-id="6fe93-121">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="6fe93-122">Gehen Sie gemäß der [Aktualisierungsanleitung](#Update) vor.</span><span class="sxs-lookup"><span data-stu-id="6fe93-122">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="6fe93-123">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6fe93-123">Update</span></span>

<span data-ttu-id="6fe93-124">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6fe93-124">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="6fe93-125">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6fe93-125">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="6fe93-126">Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="6fe93-126">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6fe93-127">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="6fe93-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6fe93-128">Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="6fe93-128">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
