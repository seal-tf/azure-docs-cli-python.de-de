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
ms.openlocfilehash: 580438bfc66f3ed0b4dad504258eab453b1b9183
ms.sourcegitcommit: c1df7794ad42adb8640b51b630e4275f4a791ac2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/19/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="84875-104">Installieren von Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="84875-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="84875-105">Installieren Sie noch heute die neue Version der Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="84875-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="84875-106">Wir haben sie verbessert und aktualisiert, um eine großartige systemeigene Befehlszeilenumgebung für die Verwaltung von Azure-Ressourcen zur Verfügung zu stellen.</span><span class="sxs-lookup"><span data-stu-id="84875-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="84875-107">Sie kann unter macOS, Linux und Windows verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="84875-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="84875-108">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="84875-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="84875-109">Wenn Sie die vorhergehende Version der Azure CLI benötigen, finden Sie hier Informationen zur [Installation der Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="84875-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="84875-110"><a name="macOS"/>Installieren unter macOS</span><span class="sxs-lookup"><span data-stu-id="84875-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="84875-111">Unter macOS können Sie die Installation mit [Homebrew](https://brew.sh/) oder manuell durchführen.</span><span class="sxs-lookup"><span data-stu-id="84875-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="84875-112">Installieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="84875-112">Install with Homebrew</span></span>

1. <span data-ttu-id="84875-113">Falls Homebrew noch nicht installiert ist, installieren Sie das Programm gemäß der [Homebrew-Installationsanweisungen](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="84875-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="84875-114">Aktualisieren Sie Ihre lokalen Homebrew-Repositorys.</span><span class="sxs-lookup"><span data-stu-id="84875-114">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="84875-115">Installieren Sie das `azure-cli`-Paket.</span><span class="sxs-lookup"><span data-stu-id="84875-115">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="84875-116">Wenn Sie zuvor die Azure CLI 1.0 mit Homebrew installiert haben, erhalten Sie die CLI 2.0 über den regulären Homebrew-Upgradeprozess und müssen nicht das Paket installieren.</span><span class="sxs-lookup"><span data-stu-id="84875-116">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="84875-117">Manuelle Installation</span><span class="sxs-lookup"><span data-stu-id="84875-117">Install manually</span></span>

1. <span data-ttu-id="84875-118">Installieren Sie die Azure CLI 2.0 mit `curl`.</span><span class="sxs-lookup"><span data-stu-id="84875-118">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="84875-119">Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="84875-119">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="84875-120">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-120">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="84875-121">Installieren unter Windows</span><span class="sxs-lookup"><span data-stu-id="84875-121">Install on Windows</span></span>

<span data-ttu-id="84875-122">Sie können die Azure CLI 2.0 über die MSI-Datei installieren und in der Windows-Befehlszeile verwenden, oder Sie können die CLI mit `apt-get` in Bash auf Ubuntu unter Windows installieren.</span><span class="sxs-lookup"><span data-stu-id="84875-122">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="84875-123">Installieren mit der MSI-Datei für die Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="84875-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="84875-124">Um die CLI unter Windows zu installieren und in der Windows-Befehlszeile zu verwenden, laden Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei herunter, und führen Sie sie aus.</span><span class="sxs-lookup"><span data-stu-id="84875-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="84875-125">Installieren mit apt-get für Bash auf Ubuntu unter Windows</span><span class="sxs-lookup"><span data-stu-id="84875-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="84875-126">Wenn Sie Bash unter Windows noch nicht haben, [installieren Sie es](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="84875-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="84875-127">Öffnen Sie die Bash-Shell.</span><span class="sxs-lookup"><span data-stu-id="84875-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="84875-128">Ändern Sie die Quellenliste.</span><span class="sxs-lookup"><span data-stu-id="84875-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="84875-129">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="84875-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="84875-130">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="84875-131">Installieren unter Debian/Ubuntu mit apt-get</span><span class="sxs-lookup"><span data-stu-id="84875-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="84875-132">Für Debian/Ubuntu-basierte Systeme können Sie Azure CLI 2.0 über `apt-get` installieren.</span><span class="sxs-lookup"><span data-stu-id="84875-132">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="84875-133">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="84875-133">Modify your sources list:</span></span>
 
   - <span data-ttu-id="84875-134">32-Bit-System</span><span class="sxs-lookup"><span data-stu-id="84875-134">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="84875-135">64-Bit-System</span><span class="sxs-lookup"><span data-stu-id="84875-135">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="84875-136">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="84875-136">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="84875-137">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-137">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="84875-138">Installieren unter RHEL, Fedora und CentOS mit yum</span><span class="sxs-lookup"><span data-stu-id="84875-138">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="84875-139">Für Distributionen, die auf Red Hat basieren und den `yum`-Paket-Manager enthalten, können Sie die Azure CLI 2.0 über `yum` installieren.</span><span class="sxs-lookup"><span data-stu-id="84875-139">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="84875-140">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="84875-140">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="84875-141">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="84875-141">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="84875-142">Aktualisieren Sie den `yum`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="84875-142">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="84875-143">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-143">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="84875-144">Installieren in OpenSUSE und SLE mit zypper</span><span class="sxs-lookup"><span data-stu-id="84875-144">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="84875-145">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="84875-145">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="84875-146">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="84875-146">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="84875-147">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="84875-147">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="84875-148">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-148">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="84875-149">Installieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="84875-149">Install with Docker</span></span>

<span data-ttu-id="84875-150">Wir behalten ein mit der Azure CLI 2.0 vorkonfiguriertes Docker-Image bei.</span><span class="sxs-lookup"><span data-stu-id="84875-150">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="84875-151">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="84875-151">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="84875-152">Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="84875-152">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="84875-153">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="84875-153">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="84875-154">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="84875-154">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="84875-155"><a name="Linux"/>Installieren unter Linux ohne apt-get</span><span class="sxs-lookup"><span data-stu-id="84875-155"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="84875-156">Es wird empfohlen, die CLI mit einen Paket-Manager zu installieren (sofern möglich).</span><span class="sxs-lookup"><span data-stu-id="84875-156">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="84875-157">Für Distributionen, für die kein Paket bereitgestellt wird, können Sie eine manuelle Installation durchführen.</span><span class="sxs-lookup"><span data-stu-id="84875-157">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="84875-158">Installieren Sie je nach Ihrer Linux-Distribution die erforderlichen Komponenten.</span><span class="sxs-lookup"><span data-stu-id="84875-158">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="84875-159">Falls Ihre Distribution oben nicht aufgeführt ist, müssen Sie [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), und [OpenSSL](https://www.openssl.org/source/) installieren.</span><span class="sxs-lookup"><span data-stu-id="84875-159">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="84875-160">Installieren Sie die CLI mit `curl`.</span><span class="sxs-lookup"><span data-stu-id="84875-160">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="84875-161">Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="84875-161">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="84875-162">Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="84875-162">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="84875-163">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="84875-163">Troubleshooting</span></span>

<span data-ttu-id="84875-164">Wenn bei der CLI-Installation ein Fehler auftritt, sehen Sie in diesem Abschnitt nach, ob Ihr Problem behandelt wird.</span><span class="sxs-lookup"><span data-stu-id="84875-164">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="84875-165">Ist das Problem hier nicht aufgeführt, melden Sie es über [Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="84875-165">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="84875-166">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="84875-166">curl "Object Moved" error</span></span>

<span data-ttu-id="84875-167">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="84875-167">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="84875-168">Deinstallieren von 1.x-Versionen der CLI</span><span class="sxs-lookup"><span data-stu-id="84875-168">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="84875-169">Wenn in Ihrem System eine ältere 1.x-Version der CLI verfügbar ist, können Sie sie basierend auf dem verwendeten Installationstyp deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="84875-169">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="84875-170">Deinstallieren mit npm</span><span class="sxs-lookup"><span data-stu-id="84875-170">Uninstall with npm</span></span>

<span data-ttu-id="84875-171">Entfernen Sie die ältere CLI mit `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="84875-171">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="84875-172">Deinstallieren mit verteilbarer Komponente</span><span class="sxs-lookup"><span data-stu-id="84875-172">Uninstall with distributable</span></span>

<span data-ttu-id="84875-173">Verwenden Sie bei der Installation über eine [MSI](http://aka.ms/webpi-azure-cli)-Datei oder ein [macOS-Paket](http://aka.ms/mac-azure-cli) das gleiche Tool zum Entfernen der Installation.</span><span class="sxs-lookup"><span data-stu-id="84875-173">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="84875-174">Deinstallieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="84875-174">Uninstall with Docker</span></span>

<span data-ttu-id="84875-175">Wenn Sie ein Docker-Image zur Verwendung der älteren CLI-Version installiert haben, entfernen Sie dieses Image und alle zugehörigen Container.</span><span class="sxs-lookup"><span data-stu-id="84875-175">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="84875-176">Sie können die Container dann nach der Installation des neuen Docker-Images neu erstellen, wie in den Installationsanweisungen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="84875-176">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="84875-177">Aktualisieren der CLI</span><span class="sxs-lookup"><span data-stu-id="84875-177">Update the CLI</span></span>

<span data-ttu-id="84875-178">Verwenden Sie zum Aktualisieren der Azure CLI die gleiche Methode wie für die Installation.</span><span class="sxs-lookup"><span data-stu-id="84875-178">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="84875-179">Aktualisieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="84875-179">Update with Homebrew</span></span>

1. <span data-ttu-id="84875-180">Aktualisieren Sie die Informationen zum lokalen Homebrew-Repository.</span><span class="sxs-lookup"><span data-stu-id="84875-180">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

2. <span data-ttu-id="84875-181">Aktualisieren Sie die installierten Pakete.</span><span class="sxs-lookup"><span data-stu-id="84875-181">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="84875-182">Aktualisieren mit der MSI-Datei</span><span class="sxs-lookup"><span data-stu-id="84875-182">Update with MSI</span></span>

<span data-ttu-id="84875-183">Führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) erneut aus.</span><span class="sxs-lookup"><span data-stu-id="84875-183">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="84875-184">Aktualisieren mit apt-get</span><span class="sxs-lookup"><span data-stu-id="84875-184">Update with apt-get</span></span>

<span data-ttu-id="84875-185">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="84875-185">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="84875-186">Dadurch werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="84875-186">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="84875-187">Um nur die CLI zu aktualisieren, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="84875-187">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="84875-188">Aktualisieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="84875-188">Update with Docker</span></span>

1. <span data-ttu-id="84875-189">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="84875-189">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="84875-190">Rufen Sie die Container ab, die derzeit das CLI-Image verwenden.</span><span class="sxs-lookup"><span data-stu-id="84875-190">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="84875-191">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="84875-191">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="84875-192">Halten Sie die Container an, und erstellen Sie sie neu.</span><span class="sxs-lookup"><span data-stu-id="84875-192">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="84875-193">Manuelles Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="84875-193">Update manually</span></span>

<span data-ttu-id="84875-194">Führen Sie zum Aktualisieren die Anweisungen für die manuelle Installation für [macOS](#macOS) oder [Linux](#Linux) aus.</span><span class="sxs-lookup"><span data-stu-id="84875-194">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="84875-195">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="84875-195">Uninstall</span></span>

<span data-ttu-id="84875-196">Es tut uns leid, wenn Sie die CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="84875-196">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="84875-197">Verwenden Sie zum Deinstallieren die gleiche Methode wie für die Installation der CLI.</span><span class="sxs-lookup"><span data-stu-id="84875-197">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="84875-198">Deinstallieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="84875-198">Uninstall with Homebrew</span></span>

<span data-ttu-id="84875-199">Deinstallieren Sie das `azure-cli`-Paket.</span><span class="sxs-lookup"><span data-stu-id="84875-199">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="84875-200">Deinstallieren mit der MSI-Datei</span><span class="sxs-lookup"><span data-stu-id="84875-200">Uninstall with MSI</span></span>

<span data-ttu-id="84875-201">Führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) noch einmal aus, und wählen Sie „Deinstallieren“.</span><span class="sxs-lookup"><span data-stu-id="84875-201">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="84875-202">Deinstallieren mit apt-get</span><span class="sxs-lookup"><span data-stu-id="84875-202">Uninstall with apt-get</span></span>

<span data-ttu-id="84875-203">Deinstallieren über `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="84875-203">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="84875-204">Deinstallieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="84875-204">Uninstall with Docker</span></span>

<span data-ttu-id="84875-205">Wenn Sie ein Docker-Image installiert haben, müssen Sie alle Container mit diesem Image entfernen und dann das lokale Image löschen.</span><span class="sxs-lookup"><span data-stu-id="84875-205">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="84875-206">Rufen Sie die Container ab, die das azure-cli-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="84875-206">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="84875-207">Löschen Sie alle Container mit dem CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="84875-207">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="84875-208">Entfernen Sie das lokal installierte CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="84875-208">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="84875-209">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="84875-209">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="84875-210">Manuelles Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="84875-210">Uninstall manually</span></span>

<span data-ttu-id="84875-211">Wenn Sie das Skript unter https://aka.ms/InstallAzureCli zum Installieren der CLI verwendet haben, können Sie sie mit diesen Schritten deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="84875-211">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="84875-212">Entfernen Sie die installierten Dateien.</span><span class="sxs-lookup"><span data-stu-id="84875-212">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="84875-213">Löschen Sie die Zeile `<install location>/lib/azure-cli/az.completion` aus `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="84875-213">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="84875-214">Das Standardinstallationsverzeichnis ist `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="84875-214">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="84875-215">Melden von CLI-Problemen und Bereitstellen von Feedback</span><span class="sxs-lookup"><span data-stu-id="84875-215">Report CLI issues and feedback</span></span>

<span data-ttu-id="84875-216">Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.</span><span class="sxs-lookup"><span data-stu-id="84875-216">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="84875-217">Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="84875-217">To provide feedback from the command line, use the `az feedback` command.</span></span>
