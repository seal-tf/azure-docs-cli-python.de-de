---
title: "Installieren der Azure-Befehlszeilenschnittstelle für macOS"
description: Installieren der Azure CLI 2.0 unter macOS
keywords: Azure CLI,Azure CLI installieren,Azure macOS, Azure installieren macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="f7dee-104">Installieren der Azure CLI 2.0 unter macOS</span><span class="sxs-lookup"><span data-stu-id="f7dee-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="f7dee-105">Bei einer macOS-Plattform können Sie die Azure CLI entweder über den [Homebrew-Paket-Manager](http://brew.sh) oder manuell installieren.</span><span class="sxs-lookup"><span data-stu-id="f7dee-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="f7dee-106">Die bevorzugte Methode ist Homebrew. Damit werden das Installieren, das Abrufen von Updates und das Deinstallieren vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="f7dee-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="f7dee-107">Installieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="f7dee-107">Use homebrew to install</span></span>

<span data-ttu-id="f7dee-108">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="f7dee-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="f7dee-109">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="f7dee-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="f7dee-110">Es ähnelt anderen Paket-Managern wie `apt` oder `yum`.</span><span class="sxs-lookup"><span data-stu-id="f7dee-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="f7dee-111">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="f7dee-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="f7dee-112">Installieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="f7dee-112">Install with homebrew</span></span>

<span data-ttu-id="f7dee-113">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="f7dee-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="f7dee-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="f7dee-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="f7dee-115">Aktualisieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="f7dee-115">Update with homebrew</span></span>

<span data-ttu-id="f7dee-116">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f7dee-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="f7dee-117">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f7dee-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="f7dee-118">Sie müssen die lokalen Repositoryinformationen und anschließend das CLI-Paket aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f7dee-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="f7dee-119">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f7dee-119">Troubleshooting</span></span>

<span data-ttu-id="f7dee-120">Ist beim Installieren oder Aktualisieren der CLI mit Homebrew ein Fehler aufgetreten?</span><span class="sxs-lookup"><span data-stu-id="f7dee-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="f7dee-121">Hier sind einige allgemeine Fehler sowie Ansätze zum Diagnostizieren und Beheben der Probleme aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f7dee-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="f7dee-122">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="f7dee-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="f7dee-123">Wenn bei der Installation Python und installierte Pakete nicht gefunden werden können, weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor, das während der Homebrew-Installation aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="f7dee-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="f7dee-124">Da die CLI nicht virtualenv verwendet, verlässt sie sich darauf, dass die richtigen, von Homebrew installierten Versionen von Python gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="f7dee-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="f7dee-125">Sie können diese Probleme vielleicht beheben, indem Sie die Python-Installation erneut verknüpfen:</span><span class="sxs-lookup"><span data-stu-id="f7dee-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="f7dee-126">Die CLI-Version ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="f7dee-126">The CLI version is out of date</span></span>

<span data-ttu-id="f7dee-127">Wenn die installierte CLI-Version Ihrer Meinung nach veraltet sein könnte, müssen Sie den Befehl `brew update` gefolgt von `brew upgrade azure-cli` ausführen.</span><span class="sxs-lookup"><span data-stu-id="f7dee-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="f7dee-128">Wenn die CLI dadurch nicht aktualisiert wird, berücksichtigen Sie, dass das Rollout von Homebrew-Paketen unter Umständen langsamer erfolgen kann als das von allgemeinen Releases.</span><span class="sxs-lookup"><span data-stu-id="f7dee-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="f7dee-129">Wenn Sie die aktuellste Version der CLI benötigen, sollten Sie sie [manuell installieren](#manage-the-cli-manually).</span><span class="sxs-lookup"><span data-stu-id="f7dee-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="f7dee-130">Deinstallieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="f7dee-130">Uninstall with homebrew</span></span>

<span data-ttu-id="f7dee-131">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="f7dee-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="f7dee-132">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="f7dee-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="f7dee-133">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="f7dee-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="f7dee-134">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f7dee-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="f7dee-135">Wenn Sie Homebrew für die Installation verwendet haben, sollten Sie Homebrew auch für die Deinstallation verwenden.</span><span class="sxs-lookup"><span data-stu-id="f7dee-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="f7dee-136">Manuelles Installieren der CLI</span><span class="sxs-lookup"><span data-stu-id="f7dee-136">Install the CLI manually</span></span>

<span data-ttu-id="f7dee-137">Wenn Sie für die Verwaltung der CLI-Installation Homebrew nicht verwenden können oder möchten, können Sie eine manuelle Installation durchführen.</span><span class="sxs-lookup"><span data-stu-id="f7dee-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="f7dee-138">Befolgen Sie die [Anweisungen für die manuelle Linux-Installation](install-azure-cli-linux.md) für die manuelle Installation unter macOS.</span><span class="sxs-lookup"><span data-stu-id="f7dee-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="f7dee-139">macOS-Version 10.9 und höhere Versionen müssen alle erforderlichen Abhängigkeiten enthalten.</span><span class="sxs-lookup"><span data-stu-id="f7dee-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>
