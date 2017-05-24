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
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a>Installieren von Azure CLI 2.0

Installieren Sie noch heute die neue Version der Azure CLI!
Wir haben sie verbessert und aktualisiert, um eine großartige systemeigene Befehlszeilenumgebung für die Verwaltung von Azure-Ressourcen zur Verfügung zu stellen.
Sie kann unter macOS, Linux und Windows verwendet werden.
Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).

> [!NOTE]
> Wenn Sie die vorhergehende Version der Azure CLI benötigen, finden Sie hier Informationen zur [Installation von Azure 1.0](/azure/cli-install-nodejs).

## <a name="macos"></a>macOS

1. Installieren Sie Azure CLI 2.0 mit einem `curl`-Befehl.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Möglicherweise müssen Sie Ihre Befehlsshell neu starten, damit einige Änderungen wirksam werden.

   ```bash
   exec -l $SHELL
   ```
   
3. Führen Sie Azure CLI 2.0 über die Eingabeaufforderung mit dem `az`-Befehl aus.

> [!Note]
> Bei der Installation mit InstallAzureCli wird `az component update` nicht unterstützt.
> Führen Sie `curl -L https://aka.ms/InstallAzureCli | bash` zum Aktualisieren auf die neueste CLI-Version erneut aus.
> 
> Informationen zum Deinstallieren finden Sie in den [Anweisungen zum manuellen Deinstallieren](#uninstall).

## <a name="windows"></a>Windows

Sie können die CLI über die MSI-Datei installieren und in der Windows-Befehlszeile verwenden, oder Sie können die CLI mit apt-get in Bash auf Ubuntu unter Windows installieren.

### <a name="msi-for-the-windows-command-line"></a>MSI-Datei für die Windows-Befehlszeile 

Um die CLI unter Windows zu installieren und in der Windows-Befehlszeile zu verwenden, laden Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei herunter, und führen Sie sie aus.

> [!NOTE]
> Bei der Installation mit der MSI-Datei wird `az component` nicht unterstützt.
> Um ein Update auf die neueste CLI durchzuführen, führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei erneut aus.
> 
> Um die CLI zu deinstallieren, führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) noch einmal aus, und wählen Sie „Deinstallieren“.

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>apt-get für Bash auf Ubuntu unter Windows

1. Wenn Sie Bash unter Windows noch nicht haben, [installieren Sie es](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Öffnen Sie die Bash-Shell.

3. Ändern Sie die Quellenliste.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Führen Sie die folgenden sudo-Befehle aus:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Bei der Installation mit apt-get wird `az component` nicht unterstützt.
> Führen Sie `sudo apt-get update && sudo apt-get install azure-cli` zum Aktualisieren der CLI erneut aus.
> 
> Zum Deinstallieren führen Sie `sudo apt-get remove azure-cli` aus.

## <a name="linux"></a>Linux

1. Unter Linux müssen Sie möglicherweise bestimmte [erforderliche Komponenten](#linux-prerequisites) installieren.

2. Installieren Sie Azure CLI 2.0 mit einem `curl`-Befehl.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Möglicherweise müssen Sie Ihre Befehlsshell neu starten, damit einige Änderungen wirksam werden.

   ```bash
   exec -l $SHELL
   ```

4. Führen Sie Azure CLI 2.0 über die Eingabeaufforderung mit dem `az`-Befehl aus.

> [!Note]
> Bei der Installation mit InstallAzureCli wird `az component update` nicht unterstützt.
> Führen Sie `curl -L https://aka.ms/InstallAzureCli | bash` zum Aktualisieren auf die neueste CLI-Version erneut aus.
> 
> Informationen zum Deinstallieren finden Sie in den [Anweisungen zum manuellen Deinstallieren](#uninstall).

## <a name="docker"></a>Docker

Wir behalten ein mit der Azure CLI vorkonfiguriertes Docker-Image bei.

Installieren Sie die Azure CLI mithilfe von `docker run`.

```bash
docker run azuresdk/azure-cli-python:<version>
```

Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

> [!NOTE]
> Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> Das Docker-Image unterstützt das [`component`-Feature](/cli/azure/component) nicht.
> Verwenden Sie zum Aktualisieren der Azure-CLI 2.0 `docker run`, um das aktuelle Image oder ein bestimmtes gewünschtes Image zu installieren.

## <a name="apt-get"></a>apt-get

Für Debian/Ubuntu-basierte Systeme können Sie Azure CLI 2.0 über `apt-get` installieren.

1. Ändern Sie die Quellenliste.

   - 32-Bit-System

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - 64-Bit-System

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Führen Sie die folgenden sudo-Befehle aus:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Bei der Installation mit apt-get wird `az component` nicht unterstützt.
> Führen Sie `sudo apt-get update && sudo apt-get install azure-cli` zum Aktualisieren der CLI erneut aus.
> 
> Zum Deinstallieren führen Sie `sudo apt-get remove azure-cli` aus.

## <a name="linux-prerequisites"></a>Linux-Voraussetzungen

1. Installieren Sie [Python](https://www.python.org/downloads), falls Sie es noch nicht haben.

2. Installieren Sie je nach Ihrer Linux-Distribution die erforderlichen Komponenten.

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

## <a name="troubleshooting"></a>Problembehandlung

### <a name="errors-with-curl-redirection"></a>Fehler bei der CURL-Umleitung

Wenn der `curl`-Befehl einen Fehler im Zusammenhang mit dem `-L`-Parameter oder den Fehler „Objekt verschoben“ zurückgibt, versuchen Sie, die vollständige URL anstatt der aka.ms-URL zu verwenden:

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

## <a name="uninstall"></a>Deinstallieren

Wenn Sie das Skript unter https://aka.ms/InstallAzureCli zum Installieren der CLI verwendet haben, können Sie sie mit diesen Schritten deinstallieren.

1. Entfernen Sie die installierten Dateien.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Löschen Sie die Zeile `<install location>/lib/azure-cli/az.completion` aus `<install location>/.bash_profile`.

> [!Note]
> Das Standardinstallationsverzeichnis ist `/Users/<username>`.

Wenn Sie die CLI mithilfe von apt-get, Docker oder der MSI-Datei installiert haben, verwenden Sie dasselbe Tool für die Deinstallation.

## <a name="reporting-issues-and-feedback"></a>Melden von Problemen und Bereitstellen von Feedback

Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.
Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.
