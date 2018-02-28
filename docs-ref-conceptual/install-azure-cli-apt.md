---
title: Installieren der Azure CLI 2.0 unter Linux mit apt
description: Installieren der Azure CLI 2.0 mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 840e5e7d6531fe92d30235f621e381589266d1d3
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2018
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

2. Führen Sie die folgenden sudo-Befehle aus:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Sie können die Azure CLI mit dem Befehl `az` ausführen.

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können. Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).

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
