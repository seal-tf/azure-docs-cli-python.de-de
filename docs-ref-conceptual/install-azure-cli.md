---
title: Installieren der Azure CLI 2.0
description: "Referenzdokumentation für die Installation der Azure CLI 2.0"
keywords: Azure CLI 2.0, Azure CLI 2.0-Referenz, Azure CLI 2.0 installieren, Azure Python CLI, Azure CLI 2.0 deinstallieren, Azure CLI, Azure CLI installieren, Azure CLI-Referenz
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
ms.openlocfilehash: 00d5b555975007d7e57f04ce5d69f4f29e6d0219
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2017
---
# <a name="install-azure-cli-20"></a>Installieren von Azure CLI 2.0

Installieren Sie noch heute die neue Version der Azure CLI!
Wir haben sie verbessert und aktualisiert, um eine großartige systemeigene Befehlszeilenumgebung für die Verwaltung von Azure-Ressourcen zur Verfügung zu stellen.
Sie kann unter macOS, Linux und Windows verwendet werden.
Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).

> [!NOTE]
> Wenn Sie die vorhergehende Version der Azure CLI benötigen, finden Sie hier Informationen zur [Installation der Azure CLI 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Installieren unter macOS

1. Installieren Sie die Azure CLI 2.0 mit `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.

   ```bash
   exec -l $SHELL
   ```
   
3. Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.

## <a name="install-on-windows"></a>Installieren unter Windows

Sie können die Azure CLI 2.0 über die MSI-Datei installieren und in der Windows-Befehlszeile verwenden, oder Sie können die CLI mit `apt-get` in Bash auf Ubuntu unter Windows installieren.

### <a name="install-with-msi-for-the-windows-command-line"></a>Installieren mit der MSI-Datei für die Windows-Befehlszeile 

Um die CLI unter Windows zu installieren und in der Windows-Befehlszeile zu verwenden, laden Sie die [MSI](https://aka.ms/InstallAzureCliWindows)-Datei herunter, und führen Sie sie aus.

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Installieren mit apt-get für Bash auf Ubuntu unter Windows

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

5.  Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.

## <a name="install-on-debianubuntu-with-apt-get"></a>Installieren unter Debian/Ubuntu mit apt-get

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

3.  Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.

## <a name="install-with-docker"></a>Installieren mit Docker

Wir behalten ein mit der Azure CLI 2.0 vorkonfiguriertes Docker-Image bei.

Installieren Sie die CLI mit `docker run`.

  ```bash
  docker run azuresdk/azure-cli-python:<version>
  ```

Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.

> [!NOTE]
> Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><a name="Linux"/>Installieren unter Linux ohne apt-get

Es wird empfohlen, die CLI mit `apt-get` zu installieren (sofern möglich). Für Distributionen, die nicht den `apt`-Paket-Manager verwenden, können Sie eine manuelle Installation durchführen.

1. Installieren Sie je nach Ihrer Linux-Distribution die erforderlichen Komponenten.

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

Falls Ihre Distribution oben nicht aufgeführt ist, müssen Sie [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), und [OpenSSL](https://www.openssl.org/source/) installieren.

2. Installieren Sie die CLI mit `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Möglicherweise müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.

   ```bash
   exec -l $SHELL
   ```

4. Führen Sie die CLI über die Eingabeaufforderung mit dem `az`-Befehl aus.

## <a name="troubleshooting"></a>Problembehandlung

Wenn bei der CLI-Installation ein Fehler auftritt, sehen Sie in diesem Abschnitt nach, ob Ihr Problem behandelt wird. Ist das Problem hier nicht aufgeführt, melden Sie es über [Github](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>curl-Fehler „Objekt verschoben“

Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a>Von Homebrew wird unter macOS eine ältere Version installiert.

Die für macOS verfügbare Homebrew-`azure-cli`-Formel ist derzeit veraltet und installiert eine 1.x-Version der CLI. Den Aktualisierungsstatus können Sie mithilfe von `brew info azure-cli` überprüfen.

[Deinstallieren Sie bis dahin die ältere Version](#uninstall_brew), und befolgen Sie die [Installationsanweisungen für macOS](#macOS).

## <a name="uninstall-cli-1x-versions"></a>Deinstallieren von 1.x-Versionen der CLI

Wenn in Ihrem System eine ältere 1.x-Version der CLI verfügbar ist, können Sie sie basierend auf dem verwendeten Installationstyp deinstallieren.

### <a name="uninstall-with-npm"></a>Deinstallieren mit npm

Entfernen Sie die ältere CLI mit `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><a name="uninstall_brew"/>Deinstallieren mit Homebrew unter macOS

Entfernen Sie die ältere CLI mit `brew uninstall`.

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a>Deinstallieren mit verteilbarer Komponente

Verwenden Sie bei der Installation über eine [MSI](http://aka.ms/webpi-azure-cli)-Datei oder ein [macOS-Paket](http://aka.ms/mac-azure-cli) das gleiche Tool zum Entfernen der Installation.

### <a name="uninstall-with-docker"></a>Deinstallieren mit Docker

Wenn Sie ein Docker-Image zur Verwendung der älteren CLI-Version installiert haben, entfernen Sie dieses Image und alle zugehörigen Container. Sie können die Container dann nach der Installation des neuen Docker-Images neu erstellen, wie in den Installationsanweisungen beschrieben.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Aktualisieren der CLI

Verwenden Sie zum Aktualisieren der Azure CLI die gleiche Methode wie für die Installation.

### <a name="update-with-msi"></a>Aktualisieren mit der MSI-Datei

Führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) erneut aus.

### <a name="update-with-apt-get"></a>Aktualisieren mit apt-get

Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Dadurch werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.
> Um nur die CLI zu aktualisieren, verwenden Sie `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a>Aktualisieren mit Docker

1. Aktualisieren Sie Ihr lokales Image mit `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Rufen Sie die Container ab, die derzeit das CLI-Image verwenden.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.

3. Halten Sie die Container an, und erstellen Sie sie neu.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>Manuelles Aktualisieren

Führen Sie zum Aktualisieren die Anweisungen für die manuelle Installation für [macOS](#macOS) oder [Linux](#Linux) aus.

## <a name="uninstall"></a>Deinstallieren

Es tut uns leid, wenn Sie die CLI deinstallieren möchten. Verwenden Sie zum Deinstallieren die gleiche Methode wie für die Installation der CLI.

### <a name="uninstall-with-msi"></a>Deinstallieren mit der MSI-Datei

Führen Sie die [MSI](https://aka.ms/InstallAzureCliWindows) noch einmal aus, und wählen Sie „Deinstallieren“.

### <a name="uninstall-with-apt-get"></a>Deinstallieren mit apt-get

Deinstallieren über `apt-get remove`:

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a>Deinstallieren mit Docker

Wenn Sie ein Docker-Image installiert haben, müssen Sie alle Container mit diesem Image entfernen und dann das lokale Image löschen.

1. Rufen Sie die Container ab, die das azure-cli-Image ausführen.

  ```bash
  docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
  ```

  ```output
  CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
  34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
  ```

2. Löschen Sie alle Container mit dem CLI-Image.

  ```bash
  docker rm 34a868beb2ab
  ```

3. Entfernen Sie das lokal installierte CLI-Image.

  ```bash
  docker rmi azuresdk/azure-cli-python
  ```

> [!NOTE]
> Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.

### <a name="uninstall-manually"></a>Manuelles Deinstallieren

Wenn Sie das Skript unter https://aka.ms/InstallAzureCli zum Installieren der CLI verwendet haben, können Sie sie mit diesen Schritten deinstallieren.

1. Entfernen Sie die installierten Dateien.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Löschen Sie die Zeile `<install location>/lib/azure-cli/az.completion` aus `<install location>/.bash_profile`.

> [!Note]
> Das Standardinstallationsverzeichnis ist `/Users/<username>`.

## <a name="report-cli-issues-and-feedback"></a>Melden von CLI-Problemen und Bereitstellen von Feedback

Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.
Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.
