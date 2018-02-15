---
title: "Manuelle Installation der Azure CLI 2.0 für Linux"
description: Manuelle Installation der Azure CLI 2.0 unter Linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4ab1f70308810e045b9a1d923fd809ad9848f6c6
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="409a7-103">Manuelle Installation der Azure CLI 2.0 unter Linux</span><span class="sxs-lookup"><span data-stu-id="409a7-103">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="409a7-104">Wenn in Ihrer Distribution kein Paket für die Azure CLI enthalten ist, können Sie die CLI durch Ausführen eines Installationsskripts jederzeit manuell installieren.</span><span class="sxs-lookup"><span data-stu-id="409a7-104">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="409a7-105">Es wird dringend empfohlen, einen Paket-Manager für die CLI zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="409a7-105">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="409a7-106">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="409a7-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="409a7-107">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="409a7-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="409a7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="409a7-108">Prerequisites</span></span>

<span data-ttu-id="409a7-109">Zum Installieren der CLI muss auf dem System folgende Software verfügbar sein:</span><span class="sxs-lookup"><span data-stu-id="409a7-109">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="409a7-110">Python 2.7 oder Python 3.x</span><span class="sxs-lookup"><span data-stu-id="409a7-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="409a7-111">libffi</span><span class="sxs-lookup"><span data-stu-id="409a7-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="409a7-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="409a7-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="409a7-113">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="409a7-113">Install or update</span></span>

<span data-ttu-id="409a7-114">Sie müssen eine vollständige Installation ausführen – unabhängig davon, ob die CLI installiert oder aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="409a7-114">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="409a7-115">Wenn alle erforderlichen Komponenten vorhanden sind, können Sie die CLI durch Ausführung von `curl` installieren.</span><span class="sxs-lookup"><span data-stu-id="409a7-115">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="409a7-116">Alternativ können Sie das Skript herunterladen und lokal ausführen.</span><span class="sxs-lookup"><span data-stu-id="409a7-116">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="409a7-117">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="409a7-117">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="409a7-118">Führen Sie nach der Installation die CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="409a7-118">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="409a7-119">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="409a7-119">Troubleshooting</span></span>

<span data-ttu-id="409a7-120">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="409a7-120">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="409a7-121">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="409a7-121">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="409a7-122">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="409a7-122">curl "Object Moved" error</span></span>

<span data-ttu-id="409a7-123">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="409a7-123">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="409a7-124">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="409a7-124">`az` command not found</span></span>

<span data-ttu-id="409a7-125">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="409a7-125">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="409a7-126">Ausführen</span><span class="sxs-lookup"><span data-stu-id="409a7-126">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="409a7-127">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="409a7-127">and check if the problem is resolved.</span></span>

<span data-ttu-id="409a7-128">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="409a7-128">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="409a7-129">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="409a7-129">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="409a7-130">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="409a7-130">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="409a7-131">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="409a7-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="409a7-132">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="409a7-132">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="409a7-133">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="409a7-133">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="409a7-134">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="409a7-134">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="409a7-135">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="409a7-135">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="409a7-136">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="409a7-136">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```
