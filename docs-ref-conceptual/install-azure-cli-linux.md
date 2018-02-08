---
title: "Manuelle Installation der Azure CLI 2.0 für Linux"
description: Manuelle Installation der Azure CLI 2.0 unter Linux
keywords: Azure CLI,Azure CLI installieren,Azure Linux, Azure installieren Linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d8c88d111c50a3cbb6b643a14dcd2a9773699657
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="3cbc2-104">Manuelle Installation der Azure CLI 2.0 unter Linux</span><span class="sxs-lookup"><span data-stu-id="3cbc2-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="3cbc2-105">Wenn in Ihrer Distribution kein Paket für die Azure CLI enthalten ist, können Sie die CLI durch Ausführen eines Installationsskripts jederzeit manuell installieren.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="3cbc2-106">Es wird dringend empfohlen, einen Paket-Manager für die CLI zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-106">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="3cbc2-107">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-107">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="3cbc2-108">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-108">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cbc2-109">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3cbc2-109">Prerequisites</span></span>

<span data-ttu-id="3cbc2-110">Zum Installieren der CLI muss auf dem System folgende Software verfügbar sein:</span><span class="sxs-lookup"><span data-stu-id="3cbc2-110">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="3cbc2-111">Python 2.7 oder Python 3.x</span><span class="sxs-lookup"><span data-stu-id="3cbc2-111">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="3cbc2-112">libffi</span><span class="sxs-lookup"><span data-stu-id="3cbc2-112">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="3cbc2-113">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="3cbc2-113">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="3cbc2-114">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3cbc2-114">Install or update</span></span> 

<span data-ttu-id="3cbc2-115">Sie müssen eine vollständige Installation ausführen – unabhängig davon, ob die CLI installiert oder aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-115">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="3cbc2-116">Wenn alle erforderlichen Komponenten vorhanden sind, können Sie die CLI durch Ausführung von `curl` installieren.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-116">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="3cbc2-117">Alternativ können Sie das Skript herunterladen und lokal ausführen.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-117">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="3cbc2-118">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-118">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="3cbc2-119">Führen Sie nach der Installation die CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-119">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3cbc2-120">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="3cbc2-120">Troubleshooting</span></span>

<span data-ttu-id="3cbc2-121">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-121">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="3cbc2-122">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3cbc2-122">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="3cbc2-123">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="3cbc2-123">curl "Object Moved" error</span></span>

<span data-ttu-id="3cbc2-124">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="3cbc2-124">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="3cbc2-125">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-125">`az` command not found</span></span>

<span data-ttu-id="3cbc2-126">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-126">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="3cbc2-127">Führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="3cbc2-127">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="3cbc2-128">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-128">and check if the problem is resolved.</span></span>

<span data-ttu-id="3cbc2-129">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-129">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="3cbc2-130">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-130">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="3cbc2-131">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="3cbc2-131">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="3cbc2-132">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="3cbc2-132">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="3cbc2-133">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-133">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="3cbc2-134">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-134">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="3cbc2-135">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-135">Remove the installed CLI files.</span></span>
  
  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="3cbc2-136">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="3cbc2-136">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>
  
  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="3cbc2-137">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="3cbc2-137">If using `bash` or `zsh`, reload your shell's command cache.</span></span>
  
  ```bash
  hash -r
  ```
