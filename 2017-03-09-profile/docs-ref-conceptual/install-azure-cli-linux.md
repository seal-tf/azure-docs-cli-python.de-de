---
title: "Manuelle Installation der Azure CLI 2.0 für Linux"
description: Manuelle Installation der Azure CLI 2.0 unter Linux
keywords: Azure CLI,Azure CLI installieren,Azure Linux, Azure installieren Linux
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
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="40165-104">Manuelle Installation der Azure CLI 2.0 unter Linux</span><span class="sxs-lookup"><span data-stu-id="40165-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="40165-105">Wenn in Ihrer Distribution kein Paket für die Azure CLI enthalten ist, können Sie die CLI durch Ausführen eines Installationsskripts jederzeit manuell installieren.</span><span class="sxs-lookup"><span data-stu-id="40165-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="40165-106">Sofern ein Paket verfügbar ist, ist dies jedoch stets die empfohlene Installationsmethode.</span><span class="sxs-lookup"><span data-stu-id="40165-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40165-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40165-107">Prerequisites</span></span>

<span data-ttu-id="40165-108">Zum Installieren der CLI muss auf dem System folgende Software verfügbar sein:</span><span class="sxs-lookup"><span data-stu-id="40165-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="40165-109">Python 2.7 oder Python 3.x</span><span class="sxs-lookup"><span data-stu-id="40165-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="40165-110">libffi</span><span class="sxs-lookup"><span data-stu-id="40165-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="40165-111">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="40165-111">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="40165-112">Manuelles Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="40165-112">Install or update manually</span></span>

<span data-ttu-id="40165-113">Sie müssen eine vollständige Installation ausführen – unabhängig davon, ob die CLI installiert oder aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="40165-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="40165-114">Wenn alle erforderlichen Komponenten vorhanden sind, können Sie die CLI durch Ausführung von `curl` installieren.</span><span class="sxs-lookup"><span data-stu-id="40165-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="40165-115">Wenn `curl` nicht auf Ihrem System vorhanden ist, können Sie auch das Skript herunterladen und lokal ausführen.</span><span class="sxs-lookup"><span data-stu-id="40165-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="40165-116">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="40165-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="40165-117">Führen Sie nach der Installation die CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="40165-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="40165-118">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="40165-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="40165-119">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="40165-119">curl "Object Moved" error</span></span>

<span data-ttu-id="40165-120">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="40165-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="40165-121">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="40165-121">`az` command not found</span></span>

<span data-ttu-id="40165-122">Wenn Sie nach der Installation den Befehl nicht ausführen können, müssen Sie unter Umständen den Befehlshash-Cache Ihrer Shell leeren.</span><span class="sxs-lookup"><span data-stu-id="40165-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="40165-123">Ausführen</span><span class="sxs-lookup"><span data-stu-id="40165-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="40165-124">und überprüfen, ob das Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="40165-124">and see if the problem is resolved.</span></span>

<span data-ttu-id="40165-125">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="40165-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="40165-126">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="40165-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="40165-127">Wenn Sie das Installationsskript ausgeführt haben:</span><span class="sxs-lookup"><span data-stu-id="40165-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="40165-128">Manuelles Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="40165-128">Unstinall manually</span></span>

<span data-ttu-id="40165-129">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="40165-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="40165-130">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="40165-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="40165-131">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="40165-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="40165-132">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="40165-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="40165-133">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Installationsverzeichnis löschen.</span><span class="sxs-lookup"><span data-stu-id="40165-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="40165-134">Das Installationsverzeichnis sollte zum Installationszeitpunkt ausgewählt worden sein, wenn die Installation über das Skript `https://aka.ms/InstallAzureCLI` erfolgt ist.</span><span class="sxs-lookup"><span data-stu-id="40165-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="40165-135">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="40165-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="40165-136">Entfernen Sie zunächst die installierten CLI-Dateien:</span><span class="sxs-lookup"><span data-stu-id="40165-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="40165-137">Ändern Sie anschließend die Datei `$HOME/.bash_profile`, um folgende Zeile zu entfernen:</span><span class="sxs-lookup"><span data-stu-id="40165-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="40165-138">Wenn Ihre Shell einen Befehlscache verwendet, laden Sie ihn erneut.</span><span class="sxs-lookup"><span data-stu-id="40165-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="40165-139">`bash`- und `zsh`-Benutzer müssen den folgenden Schritt ausführen:</span><span class="sxs-lookup"><span data-stu-id="40165-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```
