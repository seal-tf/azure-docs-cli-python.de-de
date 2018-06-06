---
title: Installieren der Azure CLI 2.0 unter Linux mit apt
description: Installieren der Azure CLI 2.0 mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7eb04b408f403264f3951bf663d43686601c4ab8
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/09/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Installieren der Azure CLI 2.0 mit apt

Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung. Dieses Paket wurde mit Folgendem getestet:

* Ubuntu Trusty, Xenial und Artful
* Debian Wheezy, Jessie und Stretch

## <a name="install"></a>Installieren

1. Ändern Sie die Quellenliste:

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Rufen Sie den Microsoft-Signaturschlüssel ab:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > Dieser Signaturschlüssel ist veraltet und wird Ende Mai 2018 ersetzt. Stellen Sie sicher, dass Sie auch den neuen Schlüssel installieren, um mit `apt` weiterhin Updates zu erhalten:
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. Installieren Sie das Basispaket:

   ```bash
   sudo apt-get install apt-transport-https
   ```

4. Installieren Sie die Befehlszeilenschnittstelle:

   ```bash
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Führen Sie den Befehl `az login` aus, um sich anzumelden.

```azurecli
az login
```

Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können. Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-fails-with-command-not-found"></a>Bei „lsb_release“ tritt der Fehler „Der Befehl wurde nicht gefunden.“ auf.

Beim Ausführen des Befehls `lsb_release` wird unter Umständen eine Ausgabe wie die folgende angezeigt:

```output
-bash: lsb_release: command not found
```

Fehlerursache: „lsb_release“ ist nicht installiert. Das Problem lässt sich durch Installieren des Pakets `lsb-release` beheben.

```bash
sudo apt-get install lsb-release
```

### <a name="apt-key-fails-with-no-dirmngr"></a>Fehler „No dirmngr“ beim Ausführen von „apt-key“

Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird. Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a>Keine Reaktion von „apt-key“

Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit. Für Ihre Firewall muss möglicherweise ein HTTP-Proxy für ausgehende Verbindungen verwendet werden:

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

Wenn Sie nicht wissen, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator. Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer, Kennwort und `@`-Token weg.

## <a name="update"></a>Aktualisieren

Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.
> Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Deinstallieren Sie sie mit `apt-get remove`.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Entfernen Sie alle nicht benötigten Pakete.

   ```bash
   sudo apt autoremove
   ```
