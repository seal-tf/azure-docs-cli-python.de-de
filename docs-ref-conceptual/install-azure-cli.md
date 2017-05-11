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
ms.openlocfilehash: b7c0b7c50794333b28c034de9b41f1e506053e25
ms.sourcegitcommit: 663d4188ccc4be425d3d551fe32613fafd05a764
ms.translationtype: HT
ms.contentlocale: de-DE
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

Azure CLI 2.0 unterstützt die Bash-Befehlssyntax, sodass Bash auf Ubuntu unter Windows eine hervorragende Möglichkeit zum Verwenden der CLI darstellt.
Wenn Sie Bash nicht verwenden, können Sie die CLI über die Windows-Befehlszeile installieren und verwenden.

### <a name="bash-on-ubuntu-on-windows"></a>Bash auf Ubuntu unter Windows

1. Wenn Sie Bash unter Windows noch nicht haben, [installieren Sie es](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Öffnen Sie die Bash-Shell.

3. Wenn Sie Python noch nicht haben, installieren Sie es.

   ```bash
   sudo apt-get install python3
   ```

   > [!NOTE]
   > Führen Sie `python --version` aus, um festzustellen, ob Sie Python installiert haben.

4. Ändern Sie die Quellenliste.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

5. Führen Sie die folgenden sudo-Befehle aus:

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

### <a name="windows-command-line"></a>Windows-Befehlszeile 

1. Rufen Sie die Python-Website auf, und [laden Sie Python für Windows herunter](https://www.python.org/downloads/).
   Achten Sie darauf, bei der Installation von Python die Pip-Komponente zu installieren.
   Nach Abschluss der Installation fügen Sie Python Ihrer PATH-Umgebungsvariable hinzu (das Installationsprogramm fordert Sie dazu auf).

2. Überprüfen Sie die Python-Installation an einer Eingabeaufforderung.

   ```bash
   python --version
   ```

3. Installieren Sie Azure CLI 2.0 mithilfe von `pip`.

   ```bash
   pip install --user azure-cli
   ```

4. Fügen Sie Ihrem Pfad den Ordner hinzu, der „az.bat“ enthält.
   Die `az.bat`-Datei der CLI wird entweder in `%USERPROFILE%\AppData\Roaming\Python\Scripts` oder `%USERPROFILE%\AppData\Roaming\Python\PythonXY\Scripts` installiert, wobei `XY` Ihre Python-Version ist (z.B. `%USERPROFILE%\AppData\Roaming\Python\Python27\Scripts`).
   Fügen Sie Ihrem Pfad den Ordner hinzu, der `az.bat` enthält.
   
4. Führen Sie Azure CLI 2.0 über die Eingabeaufforderung mit dem `az`-Befehl aus.

> [!NOTE]
> Wenn Sie Azure CLI 2.0 bereits installiert haben und überprüfen möchten, ob es sich um die aktuelle Version handelt, verwenden Sie dazu `az --version`.
> Vergleichen Sie Ihre Version mit der aktuellen Version unter [https://pypi.python.org/pypi/azure-cli](https://pypi.python.org/pypi/azure-cli).
> 
> Führen Sie `az component update` zum Aktualisieren auf die neueste CLI-Version aus.
> 
> Führen Sie zum Deinstallieren der CLI `pip uninstall azure-cli` aus.

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
-------------------------------

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


### <a name="errors-on-install-with-cffi-or-cryptography"></a>Fehler bei der Installation mit `cffi` oder Kryptografie

Wenn bei der Installation unter OS X Fehler auftreten, aktualisieren Sie `pip`.

```bash
pip install --upgrade --force-reinstall pip
```

Wenn bei der Installation unter **Debian** oder **Ubuntu** Fehler wie in diesen Beispielen auftreten, installieren Sie `libssl-dev` und `libffi-dev`.

```bash
sudo apt-get update
sudo apt-get install -y libssl-dev libffi-dev
```

Installieren Sie auch Python Dev für Ihre Version von Python.

Python 2:

```bash
sudo apt-get install -y python-dev
```

Python 3:

```bash
sudo apt-get install -y python3-dev
```

Ubuntu 15 erfordert möglicherweise auch `build-essential`:

```bash
sudo apt-get install -y build-essential
```

### <a name="example-errors"></a>Fehlerbeispiele

```
Downloading cffi-1.5.2.tar.gz (388kB)
    100% |################################| 389kB 3.9MB/s
    Complete output from command python setup.py egg_info:

        No working compiler found, or bogus compiler options
        passed to the compiler from Python's distutils module.
        See the error messages above.
        (If they are about -mno-fused-madd and you are on OS/X 10.8,
        see http://stackoverflow.com/questions/22313407/ .)

    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-77i2fido/cffi/
```

```
#include <openssl/e_os2.h>
                            ^
compilation terminated.
error: command 'x86_64-linux-gnu-gcc' failed with exit status 1

Failed building wheel for cryptography
```

Siehe Stack Overflow-Frage: [Failed to install Python Cryptography package with PIP and setup.py](http://stackoverflow.com/questions/22073516/failed-to-install-python-cryptography-package-with-pip-and-setup-py) (Fehler beim Installieren des Python-Kryptografiepakets mit PIP und „setup.py“)

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

Wenn Sie die CLI mithilfe von PIP, apt-get oder Docker installiert haben, verwenden Sie dasselbe Tool, um sie zu deinstallieren.

## <a name="reporting-issues-and-feedback"></a>Melden von Problemen und Bereitstellen von Feedback

Wenn mit dem Tool Fehler auftreten, legen Sie einen Eintrag im Bereich [Probleme](https://github.com/Azure/azure-cli/issues) unseres GitHub Repositorys an.
Zum Senden von Feedback über die Befehlszeile verwenden Sie den Befehl `az feedback`.
