---
title: "Installieren der Azure-Befehlszeilenschnittstelle für macOS"
description: Installieren der Azure CLI 2.0 unter macOS
keywords: Azure CLI,Azure CLI installieren,Azure macOS, Azure installieren macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 36fd2604677db0b7f820ee11884bf790fb1d75cb
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="dad7d-104">Installieren der Azure CLI 2.0 unter macOS</span><span class="sxs-lookup"><span data-stu-id="dad7d-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="dad7d-105">Bei Verwendung der macOS-Plattform können Sie die Azure CLI über den [Homebrew-Paket-Manager](http://brew.sh) installieren.</span><span class="sxs-lookup"><span data-stu-id="dad7d-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="dad7d-106">Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten.</span><span class="sxs-lookup"><span data-stu-id="dad7d-106">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="dad7d-107">Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.</span><span class="sxs-lookup"><span data-stu-id="dad7d-107">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="dad7d-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="dad7d-108">Install</span></span>

<span data-ttu-id="dad7d-109">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="dad7d-109">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="dad7d-110">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="dad7d-110">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="dad7d-111">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="dad7d-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="dad7d-112">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="dad7d-112">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="dad7d-113">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="dad7d-113">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="dad7d-114">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="dad7d-114">Troubleshooting</span></span>

<span data-ttu-id="dad7d-115">In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können.</span><span class="sxs-lookup"><span data-stu-id="dad7d-115">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="dad7d-116">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="dad7d-116">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="dad7d-117">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="dad7d-117">Unable to find Python or installed packages</span></span>

<span data-ttu-id="dad7d-118">Sollten Python oder installierte Pakete bei der Installation nicht gefunden werden, weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor, das während der Homebrew-Installation aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="dad7d-118">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="dad7d-119">Da die CLI keine virtuelle Python-Umgebung verwendet, muss sie die korrekte Python-Version finden können.</span><span class="sxs-lookup"><span data-stu-id="dad7d-119">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="dad7d-120">Zur Behebung dieser Probleme können Sie ggf. die Python-Installation neu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="dad7d-120">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="dad7d-121">CLI-Version 1.x wird installiert.</span><span class="sxs-lookup"><span data-stu-id="dad7d-121">CLI version 1.x is installed</span></span>

<span data-ttu-id="dad7d-122">Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein.</span><span class="sxs-lookup"><span data-stu-id="dad7d-122">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="dad7d-123">Gehen Sie gemäß der [Aktualisierungsanleitung](#Update) vor.</span><span class="sxs-lookup"><span data-stu-id="dad7d-123">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="dad7d-124">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dad7d-124">Update</span></span>

<span data-ttu-id="dad7d-125">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="dad7d-125">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="dad7d-126">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="dad7d-126">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="dad7d-127">Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="dad7d-127">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="dad7d-128">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="dad7d-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="dad7d-129">Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="dad7d-129">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
