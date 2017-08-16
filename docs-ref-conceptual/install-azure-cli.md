---
title: Installieren der Azure CLI 2.0
description: "Referenzdokumente für Azure CLI 2.0"
keywords: Azure CLI 2.0, Azure CLI 2.0-Referenz, Azure CLI 2.0 installieren, Azure Python CLI, Azure CLI 2.0 deinstallieren
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.contentlocale: de-DE
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="18248-104">Installieren von Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="18248-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="18248-105">Installieren Sie noch heute die neue Version der Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="18248-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="18248-106">Wir haben sie verbessert und aktualisiert, um eine großartige systemeigene Befehlszeilenumgebung für die Verwaltung von Azure-Ressourcen zur Verfügung zu stellen.</span><span class="sxs-lookup"><span data-stu-id="18248-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="18248-107">Sie kann unter macOS, Linux und Windows verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="18248-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="18248-108">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18248-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="18248-109">Wenn Sie die vorhergehende Version der Azure CLI benötigen, finden Sie hier Informationen zur [Installation von Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="18248-109">If you need the previous version of the Azure CLI, here's how to [install Azure 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="18248-110">macOS</span><span class="sxs-lookup"><span data-stu-id="18248-110">macOS</span></span>

1. <span data-ttu-id="18248-111">Installieren Sie Azure CLI 2.0 mit einem `curl`-Befehl.</span><span class="sxs-lookup"><span data-stu-id="18248-111">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="18248-112">Möglicherweise müssen Sie Ihre Befehlsshell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="18248-112">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="18248-113">Führen Sie Azure CLI 2.0 über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="18248-113">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="18248-114">Bei der Installation mit InstallAzureCli wird `az component update` nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18248-114">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="18248-115">Führen Sie `curl -L https://aka.ms/InstallAzureCli | bash` zum Aktualisieren auf die neueste CLI-Version erneut aus.</span><span class="sxs-lookup"><span data-stu-id="18248-115">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="18248-116">Informationen zum Deinstallieren finden Sie in den [Anweisungen zum manuellen Deinstallieren](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="18248-116">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="18248-117">Windows</span><span class="sxs-lookup"><span data-stu-id="18248-117">Windows</span></span>

<span data-ttu-id="18248-118">Sie können die CLI über die MSI-Datei installieren und in der Windows-Befehlszeile verwenden, oder Sie können die CLI mit apt-get in Bash auf Ubuntu unter Windows installieren.</span><span class="sxs-lookup"><span data-stu-id="18248-118">You can install the CLI with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="18248-119">MSI-Datei für die Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="18248-119">MSI for the Windows command-line</span></span> 

<span data-ttu-id="18248-120">Um die CLI unter Windows zu installieren und in der Windows-Befehlszeile zu verwenden, laden Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei herunter, und führen Sie sie aus.</span><span class="sxs-lookup"><span data-stu-id="18248-120">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="18248-121">Bei der Installation mit der MSI-Datei wird `az component` nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18248-121">When you install with the msi, `az component` isn't supported.</span></span>
> <span data-ttu-id="18248-122">Um ein Update auf die neueste CLI durchzuführen, führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei erneut aus.</span><span class="sxs-lookup"><span data-stu-id="18248-122">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="18248-123">Um die CLI zu deinstallieren, führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) noch einmal aus, und wählen Sie „Deinstallieren“.</span><span class="sxs-lookup"><span data-stu-id="18248-123">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="18248-124">apt-get für Bash auf Ubuntu unter Windows</span><span class="sxs-lookup"><span data-stu-id="18248-124">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="18248-125">Wenn Sie Bash unter Windows noch nicht haben, [installieren Sie es](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="18248-125">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="18248-126">Öffnen Sie die Bash-Shell.</span><span class="sxs-lookup"><span data-stu-id="18248-126">Open the Bash shell.</span></span>

3. <span data-ttu-id="18248-127">Ändern Sie die Quellenliste.</span><span class="sxs-lookup"><span data-stu-id="18248-127">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="18248-128">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="18248-128">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="18248-129">Bei der Installation mit apt-get wird `az component` nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18248-129">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="18248-130">Führen Sie `sudo apt-get update && sudo apt-get install azure-cli` zum Aktualisieren der CLI erneut aus.</span><span class="sxs-lookup"><span data-stu-id="18248-130">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="18248-131">Zum Deinstallieren führen Sie `sudo apt-get remove azure-cli` aus.</span><span class="sxs-lookup"><span data-stu-id="18248-131">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux"></a><span data-ttu-id="18248-132">Linux</span><span class="sxs-lookup"><span data-stu-id="18248-132">Linux</span></span>

1. <span data-ttu-id="18248-133">Unter Linux müssen Sie möglicherweise bestimmte [erforderliche Komponenten](#linux-prerequisites) installieren.</span><span class="sxs-lookup"><span data-stu-id="18248-133">On Linux, you may need to install specific [prerequisites](#linux-prerequisites).</span></span>

2. <span data-ttu-id="18248-134">Installieren Sie Azure CLI 2.0 mit einem `curl`-Befehl.</span><span class="sxs-lookup"><span data-stu-id="18248-134">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="18248-135">Möglicherweise müssen Sie Ihre Befehlsshell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="18248-135">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="18248-136">Führen Sie Azure CLI 2.0 über die Eingabeaufforderung mit dem `az`-Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="18248-136">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="18248-137">Bei der Installation mit InstallAzureCli wird `az component update` nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18248-137">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="18248-138">Führen Sie `curl -L https://aka.ms/InstallAzureCli | bash` zum Aktualisieren auf die neueste CLI-Version erneut aus.</span><span class="sxs-lookup"><span data-stu-id="18248-138">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="18248-139">Informationen zum Deinstallieren finden Sie in den [Anweisungen zum manuellen Deinstallieren](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="18248-139">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="docker"></a><span data-ttu-id="18248-140">Docker</span><span class="sxs-lookup"><span data-stu-id="18248-140">Docker</span></span>

<span data-ttu-id="18248-141">Wir behalten ein mit der Azure CLI vorkonfiguriertes Docker-Image bei.</span><span class="sxs-lookup"><span data-stu-id="18248-141">We maintain a Docker image preconfigured with the Azure CLI.</span></span>

<span data-ttu-id="18248-142">Installieren Sie die Azure CLI mithilfe von `docker run`.</span><span class="sxs-lookup"><span data-stu-id="18248-142">Install the Azure CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="18248-143">Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="18248-143">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="18248-144">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="18248-144">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> <span data-ttu-id="18248-145">Das Docker-Image unterstützt das [`component`-Feature](/cli/azure/component) nicht.</span><span class="sxs-lookup"><span data-stu-id="18248-145">The Docker image does not support the [`component` feature](/cli/azure/component).</span></span>
> <span data-ttu-id="18248-146">Verwenden Sie zum Aktualisieren der Azure-CLI 2.0 `docker run`, um das aktuelle Image oder ein bestimmtes gewünschtes Image zu installieren.</span><span class="sxs-lookup"><span data-stu-id="18248-146">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="apt-get"></a><span data-ttu-id="18248-147">apt-get</span><span class="sxs-lookup"><span data-stu-id="18248-147">apt-get</span></span>

<span data-ttu-id="18248-148">Für Debian/Ubuntu-basierte Systeme können Sie Azure CLI 2.0 über `apt-get` installieren.</span><span class="sxs-lookup"><span data-stu-id="18248-148">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="18248-149">Ändern Sie die Quellenliste.</span><span class="sxs-lookup"><span data-stu-id="18248-149">Modify your sources list.</span></span>

   - <span data-ttu-id="18248-150">32-Bit-System</span><span class="sxs-lookup"><span data-stu-id="18248-150">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="18248-151">64-Bit-System</span><span class="sxs-lookup"><span data-stu-id="18248-151">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="18248-152">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="18248-152">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="18248-153">Bei der Installation mit apt-get wird `az component` nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18248-153">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="18248-154">Führen Sie `sudo apt-get update && sudo apt-get install azure-cli` zum Aktualisieren der CLI erneut aus.</span><span class="sxs-lookup"><span data-stu-id="18248-154">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="18248-155">Zum Deinstallieren führen Sie `sudo apt-get remove azure-cli` aus.</span><span class="sxs-lookup"><span data-stu-id="18248-155">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux-prerequisites"></a><span data-ttu-id="18248-156">Linux-Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18248-156">Linux Prerequisites</span></span>

1. <span data-ttu-id="18248-157">Installieren Sie [Python](https://www.python.org/downloads), falls Sie es noch nicht haben.</span><span class="sxs-lookup"><span data-stu-id="18248-157">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="18248-158">Installieren Sie je nach Ihrer Linux-Distribution die erforderlichen Komponenten.</span><span class="sxs-lookup"><span data-stu-id="18248-158">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a><span data-ttu-id="18248-159">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="18248-159">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="18248-160">Fehler bei der CURL-Umleitung</span><span class="sxs-lookup"><span data-stu-id="18248-160">Errors with curl redirection</span></span>

<span data-ttu-id="18248-161">Wenn der `curl`-Befehl einen Fehler im Zusammenhang mit dem `-L`-Parameter oder den Fehler „Objekt verschoben“ zurückgibt, versuchen Sie, die vollständige URL anstatt der aka.ms-URL zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="18248-161">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="18248-162">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="18248-162">Uninstall</span></span>

<span data-ttu-id="18248-163">Wenn Sie das Skript unter https://aka.ms/InstallAzureCli zum Installieren der CLI verwendet haben, können Sie sie mit diesen Schritten deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="18248-163">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="18248-164">Entfernen Sie die installierten Dateien.</span><span class="sxs-lookup"><span data-stu-id="18248-164">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="18248-165">Löschen Sie die Zeile `<install location>/lib/azure-cli/az.completion` aus `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="18248-165">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="18248-166">Das Standardinstallationsverzeichnis ist `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="18248-166">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="18248-167">Wenn Sie die CLI mithilfe von apt-get, Docker oder der MSI-Datei installiert haben, verwenden Sie dasselbe Tool für die Deinstallation.</span><span class="sxs-lookup"><span data-stu-id="18248-167">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="18248-168">Melden von Problemen und Bereitstellen von Feedback</span><span class="sxs-lookup"><span data-stu-id="18248-168">Reporting issues and feedback</span></span>

<span data-ttu-id="18248-169">Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.</span><span class="sxs-lookup"><span data-stu-id="18248-169">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="18248-170">Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="18248-170">To provide feedback from the command line, try the `az feedback` command.</span></span>
