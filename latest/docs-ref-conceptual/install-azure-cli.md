---
title: Installieren der Azure CLI 2.0
description: "Referenzdokumentation für die Installation der Azure CLI 2.0"
keywords: Azure CLI,Azure CLI installieren,Azure Python CLI,Azure CLI-Referenz
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 4703a192e23b04d0ad42daf60e415d798610cce0
ms.sourcegitcommit: 932cc86172ab55c00346f62504787c096ed7b2bd
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/24/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="d629b-104">Installieren von Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d629b-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="d629b-105">Installieren Sie noch heute die neue Version der Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="d629b-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="d629b-106">Wir haben sie verbessert und aktualisiert, um eine großartige systemeigene Befehlszeilenumgebung für die Verwaltung von Azure-Ressourcen zur Verfügung zu stellen.</span><span class="sxs-lookup"><span data-stu-id="d629b-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="d629b-107">Sie kann unter macOS, Linux und Windows verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d629b-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="d629b-108">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d629b-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="d629b-109">Wenn Sie die vorhergehende Version der Azure CLI benötigen, finden Sie hier Informationen zur [Installation der Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="d629b-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="d629b-110"><a name="macOS"/>Installieren unter macOS</span><span class="sxs-lookup"><span data-stu-id="d629b-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="d629b-111">Unter macOS können Sie die Installation mit [Homebrew](https://brew.sh/) oder manuell durchführen.</span><span class="sxs-lookup"><span data-stu-id="d629b-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="d629b-112">Installieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="d629b-112">Install with Homebrew</span></span>

1. <span data-ttu-id="d629b-113">Falls Homebrew noch nicht installiert ist, installieren Sie das Programm gemäß der [Homebrew-Installationsanweisungen](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="d629b-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="d629b-114">Wenn Sie die CLI zuvor manuell installiert haben, befolgen Sie die Anweisungen zur [manuellen Deinstallation](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="d629b-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="d629b-115">Aktualisieren Sie Ihre lokalen Homebrew-Repositorys.</span><span class="sxs-lookup"><span data-stu-id="d629b-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="d629b-116">Installieren Sie das `azure-cli`-Paket.</span><span class="sxs-lookup"><span data-stu-id="d629b-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="d629b-117">Wenn Sie zuvor die Azure CLI 1.0 mit Homebrew installiert haben, erhalten Sie die CLI 2.0 über den regulären Homebrew-Upgradeprozess und müssen nicht das Paket installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="d629b-118">Manuelle Installation</span><span class="sxs-lookup"><span data-stu-id="d629b-118">Install manually</span></span>

1. <span data-ttu-id="d629b-119">Installieren Sie die Azure CLI 2.0 mit `curl`.</span><span class="sxs-lookup"><span data-stu-id="d629b-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="d629b-120">Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="d629b-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="d629b-121">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="d629b-122">Installieren unter Windows</span><span class="sxs-lookup"><span data-stu-id="d629b-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="d629b-123">Installieren mit der MSI-Datei für die Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="d629b-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="d629b-124">Um die CLI unter Windows zu installieren und in der Windows-Befehlszeile zu verwenden, laden Sie den [Azure CLI-Installer (MSI)](https://aka.ms/InstallAzureCliWindows) herunter, und führen Sie ihn aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="d629b-125">Installieren mit apt-get für Bash auf Ubuntu unter Windows</span><span class="sxs-lookup"><span data-stu-id="d629b-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="d629b-126">Wenn Sie Bash unter Windows noch nicht haben, [installieren Sie es](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="d629b-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="d629b-127">Öffnen Sie die Bash-Shell.</span><span class="sxs-lookup"><span data-stu-id="d629b-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="d629b-128">Ändern Sie die Quellenliste.</span><span class="sxs-lookup"><span data-stu-id="d629b-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="d629b-129">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="d629b-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="d629b-130">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="d629b-131">Installieren unter Debian/Ubuntu mit apt-get</span><span class="sxs-lookup"><span data-stu-id="d629b-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="d629b-132">Für Distributionen, die den `apt`-Paket-Manager verwenden, können Sie Azure CLI 2.0 über `apt-get` installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-132">For distributions using the `apt` package manager, you can install Azure CLI 2.0 via `apt-get`.</span></span>

> [!NOTE]
> <span data-ttu-id="d629b-133">Ihre Distribution muss Python 2.7.x oder Python 3.x unterstützen, damit die CLI verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d629b-133">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="d629b-134">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="d629b-134">Modify your sources list:</span></span>
 
   - <span data-ttu-id="d629b-135">32-Bit-System</span><span class="sxs-lookup"><span data-stu-id="d629b-135">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="d629b-136">64-Bit-System</span><span class="sxs-lookup"><span data-stu-id="d629b-136">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="d629b-137">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="d629b-137">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="d629b-138">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-138">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="d629b-139">Installieren unter RHEL, Fedora und CentOS mit yum</span><span class="sxs-lookup"><span data-stu-id="d629b-139">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="d629b-140">Für Distributionen, die den `yum`-Paket-Manager verwenden, können Sie Azure CLI 2.0 über `yum` installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-140">For distributions which use the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

> [!NOTE]
> <span data-ttu-id="d629b-141">Ihre Distribution muss Python 2.7.x oder Python 3.x unterstützen, damit die CLI verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d629b-141">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="d629b-142">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="d629b-142">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="d629b-143">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="d629b-143">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="d629b-144">Aktualisieren Sie den `yum`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="d629b-144">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="d629b-145">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-145">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="d629b-146">Installieren in OpenSUSE und SLE mit zypper</span><span class="sxs-lookup"><span data-stu-id="d629b-146">Install on openSUSE and SLE with zypper</span></span>

<span data-ttu-id="d629b-147">Für Distributionen, die den `zypper`-Paket-Manager verwenden, können Sie Azure CLI 2.0 über `zypper` installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-147">For distributions which use the `zypper` package manager, you can install Azure CLI 2.0 via `zypper`.</span></span>

> [!NOTE]
> <span data-ttu-id="d629b-148">Ihre Distribution muss Python 2.7.x oder Python 3.x unterstützen, damit die CLI verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d629b-148">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="d629b-149">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="d629b-149">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="d629b-150">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="d629b-150">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="d629b-151">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="d629b-151">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="d629b-152">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-152">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="d629b-153">Installieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="d629b-153">Install with Docker</span></span>

<span data-ttu-id="d629b-154">Wir behalten ein mit der Azure CLI 2.0 vorkonfiguriertes Docker-Image bei.</span><span class="sxs-lookup"><span data-stu-id="d629b-154">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="d629b-155">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="d629b-155">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="d629b-156">Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="d629b-156">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="d629b-157">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="d629b-157">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="d629b-158">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="d629b-158">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="d629b-159"><a name="Linux"/>Installieren unter Linux ohne Paket-Manager</span><span class="sxs-lookup"><span data-stu-id="d629b-159"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="d629b-160">Es wird empfohlen, die CLI mit einen Paket-Manager zu installieren (sofern möglich).</span><span class="sxs-lookup"><span data-stu-id="d629b-160">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="d629b-161">Falls Sie die Repositorys von Microsoft nicht hinzufügen möchten oder eine Distribution ohne bereitgestelltes Paket verwenden, können Sie die CLI manuell installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-161">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="d629b-162">Installieren Sie je nach Ihrer Linux-Distribution die erforderlichen Komponenten.</span><span class="sxs-lookup"><span data-stu-id="d629b-162">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="d629b-163">Falls Ihre Distribution oben nicht aufgeführt ist, müssen Sie [Python 2.7 oder höher](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) und [OpenSSL](https://www.openssl.org/source/) installieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-163">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="d629b-164">Installieren Sie die CLI mit `curl`.</span><span class="sxs-lookup"><span data-stu-id="d629b-164">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="d629b-165">Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="d629b-165">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="d629b-166">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-166">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d629b-167">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="d629b-167">Troubleshooting</span></span>

<span data-ttu-id="d629b-168">Wenn bei der CLI-Installation ein Fehler auftritt, sehen Sie in diesem Abschnitt nach, ob Ihr Problem behandelt wird.</span><span class="sxs-lookup"><span data-stu-id="d629b-168">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="d629b-169">Ist das Problem hier nicht aufgeführt, melden Sie es über [Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d629b-169">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="d629b-170">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="d629b-170">curl "Object Moved" error</span></span>

<span data-ttu-id="d629b-171">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="d629b-171">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="d629b-172">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="d629b-172">`az` command not found</span></span>

<span data-ttu-id="d629b-173">Unter Umständen müssen Sie den Befehlshash-Cache Ihrer Shell leeren.</span><span class="sxs-lookup"><span data-stu-id="d629b-173">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="d629b-174">Ausführen</span><span class="sxs-lookup"><span data-stu-id="d629b-174">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="d629b-175">und überprüfen, ob das Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="d629b-175">and see if the problem is resolved.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="d629b-176">Deinstallieren von 1.x-Versionen der CLI</span><span class="sxs-lookup"><span data-stu-id="d629b-176">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="d629b-177">Wenn in Ihrem System eine ältere 1.x-Version der CLI verfügbar ist, können Sie sie basierend auf dem verwendeten Installationstyp deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-177">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="d629b-178">Deinstallieren mit npm</span><span class="sxs-lookup"><span data-stu-id="d629b-178">Uninstall with npm</span></span>

<span data-ttu-id="d629b-179">Entfernen Sie die ältere CLI mit `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="d629b-179">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="d629b-180">Deinstallieren mit verteilbarer Komponente</span><span class="sxs-lookup"><span data-stu-id="d629b-180">Uninstall with distributable</span></span>

<span data-ttu-id="d629b-181">Verwenden Sie bei der Installation über den [Azure CLI-Installer (MSI)](http://aka.ms/webpi-azure-cli) oder ein [macOS-Paket](http://aka.ms/mac-azure-cli) das gleiche Tool zum Entfernen der Installation.</span><span class="sxs-lookup"><span data-stu-id="d629b-181">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="d629b-182">Deinstallieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="d629b-182">Uninstall with Docker</span></span>

<span data-ttu-id="d629b-183">Wenn Sie ein Docker-Image zur Verwendung der älteren CLI-Version installiert haben, entfernen Sie dieses Image und alle zugehörigen Container.</span><span class="sxs-lookup"><span data-stu-id="d629b-183">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="d629b-184">Sie können die Container dann nach der Installation des neuen Docker-Images neu erstellen, wie in den Installationsanweisungen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="d629b-184">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="d629b-185">Aktualisieren der CLI</span><span class="sxs-lookup"><span data-stu-id="d629b-185">Update the CLI</span></span>

<span data-ttu-id="d629b-186">Verwenden Sie zum Aktualisieren der Azure CLI die gleiche Methode wie für die Installation.</span><span class="sxs-lookup"><span data-stu-id="d629b-186">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="d629b-187">Aktualisieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="d629b-187">Update with Homebrew</span></span>

1. <span data-ttu-id="d629b-188">Falls Sie zuvor die manuelle Installation durchgeführt haben, befolgen Sie die Anweisungen zum [Installieren mit Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="d629b-188">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="d629b-189">Aktualisieren Sie die Informationen zum lokalen Homebrew-Repository.</span><span class="sxs-lookup"><span data-stu-id="d629b-189">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="d629b-190">Aktualisieren Sie die installierten Pakete.</span><span class="sxs-lookup"><span data-stu-id="d629b-190">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="d629b-191">Aktualisieren mit der MSI-Datei</span><span class="sxs-lookup"><span data-stu-id="d629b-191">Update with MSI</span></span>

<span data-ttu-id="d629b-192">Führen Sie den [Azure CLI-Installer (MSI)](https://aka.ms/InstallAzureCliWindows) erneut aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-192">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="d629b-193">Aktualisieren mit apt-get</span><span class="sxs-lookup"><span data-stu-id="d629b-193">Update with apt-get</span></span>

<span data-ttu-id="d629b-194">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="d629b-194">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="d629b-195">Dadurch werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="d629b-195">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="d629b-196">Um nur die CLI zu aktualisieren, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="d629b-196">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="d629b-197">Aktualisieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="d629b-197">Update with Docker</span></span>

1. <span data-ttu-id="d629b-198">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="d629b-198">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="d629b-199">Rufen Sie die Container ab, die derzeit das CLI-Image verwenden.</span><span class="sxs-lookup"><span data-stu-id="d629b-199">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="d629b-200">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="d629b-200">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="d629b-201">Halten Sie die Container an, und erstellen Sie sie neu.</span><span class="sxs-lookup"><span data-stu-id="d629b-201">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="d629b-202">Manuelles Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d629b-202">Update manually</span></span>

<span data-ttu-id="d629b-203">Führen Sie zum Aktualisieren die Anweisungen für die manuelle Installation für [macOS](#macOS) oder [Linux](#Linux) aus.</span><span class="sxs-lookup"><span data-stu-id="d629b-203">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="d629b-204">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d629b-204">Uninstall</span></span>

<span data-ttu-id="d629b-205">Es tut uns leid, wenn Sie die CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="d629b-205">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="d629b-206">Verwenden Sie zum Deinstallieren die gleiche Methode wie für die Installation der CLI.</span><span class="sxs-lookup"><span data-stu-id="d629b-206">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="d629b-207">Deinstallieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="d629b-207">Uninstall with Homebrew</span></span>

<span data-ttu-id="d629b-208">Deinstallieren Sie das `azure-cli`-Paket.</span><span class="sxs-lookup"><span data-stu-id="d629b-208">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="d629b-209">Deinstallieren mit der MSI-Datei</span><span class="sxs-lookup"><span data-stu-id="d629b-209">Uninstall with MSI</span></span>

<span data-ttu-id="d629b-210">Führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) noch einmal aus, und wählen Sie „Deinstallieren“.</span><span class="sxs-lookup"><span data-stu-id="d629b-210">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="d629b-211">Deinstallieren mit apt-get</span><span class="sxs-lookup"><span data-stu-id="d629b-211">Uninstall with apt-get</span></span>

<span data-ttu-id="d629b-212">Deinstallieren über `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="d629b-212">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="d629b-213">Deinstallieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="d629b-213">Uninstall with Docker</span></span>

<span data-ttu-id="d629b-214">Wenn Sie ein Docker-Image installiert haben, müssen Sie alle Container mit diesem Image entfernen und dann das lokale Image löschen.</span><span class="sxs-lookup"><span data-stu-id="d629b-214">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="d629b-215">Rufen Sie die Container ab, die das azure-cli-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="d629b-215">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="d629b-216">Löschen Sie alle Container mit dem CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="d629b-216">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="d629b-217">Entfernen Sie das lokal installierte CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="d629b-217">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="d629b-218">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="d629b-218">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="d629b-219"><a name="UninstallManually"/>Manuelles Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d629b-219"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="d629b-220">Wenn Sie das Skript unter https://aka.ms/InstallAzureCli zum Installieren der CLI verwendet haben, können Sie sie mit diesen Schritten deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="d629b-220">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="d629b-221">Entfernen Sie die installierten Dateien.</span><span class="sxs-lookup"><span data-stu-id="d629b-221">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="d629b-222">Löschen Sie die Zeile `<install location>/lib/azure-cli/az.completion` aus `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="d629b-222">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="d629b-223">Wenn Ihre Shell einen Befehlscache verwendet, laden Sie ihn erneut.</span><span class="sxs-lookup"><span data-stu-id="d629b-223">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="d629b-224">Das Standardinstallationsverzeichnis ist `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="d629b-224">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="d629b-225">Melden von CLI-Problemen und Bereitstellen von Feedback</span><span class="sxs-lookup"><span data-stu-id="d629b-225">Report CLI issues and feedback</span></span>

<span data-ttu-id="d629b-226">Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.</span><span class="sxs-lookup"><span data-stu-id="d629b-226">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="d629b-227">Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="d629b-227">To provide feedback from the command line, use the `az feedback` command.</span></span>
