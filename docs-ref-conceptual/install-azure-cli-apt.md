---
title: Installieren der Azure CLI 2.0 mit apt
description: Installieren der Azure CLI 2.0 mit dem apt-Paket-Manager
keywords: Azure CLI,Azure CLI installieren,Azure apt, Azure Debian, Azure Ubuntu
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
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Installieren der Azure CLI 2.0 mit apt

Wenn Sie eine Distribution ausführen, in der `apt` enthalten ist (etwa Ubuntu oder Debian), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installieren

1. Ändern Sie die Quellenliste:

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
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Sie können die Azure CLI mit dem Befehl `az` ausführen.

## <a name="update"></a>Aktualisieren

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

### <a name="uninstall"></a>Deinstallieren

Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten. Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können. Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist. Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).

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
