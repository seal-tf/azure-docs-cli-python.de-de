---
title: Installieren der Azure CLI 2.0 unter Linux mit zypper
description: Installieren der Azure CLI 2.0 mit zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dde90e78f3ec53d323ca78c816ceefb8cf65608b
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>Installieren der Azure CLI 2.0 mit zypper

Wenn Sie eine Distribution mit `zypper` verwenden (etwa openSUSE oder SLES), steht ein Paket für die Azure CLI zur Verfügung. Dieses Paket wurde mit openSUSE 42.2 und SLES 12 SP 2 getestet.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installieren

1. Installieren Sie `curl`:

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Importieren Sie den Microsoft-Repositoryschlüssel:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Erstellen Sie lokale `azure-cli`-Repositoryinformationen:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:

   ```bash
   sudo zypper refresh
   sudo zypper install --from azure-cli -y azure-cli
   ```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Führen Sie den Befehl `az login` aus, um sich anzumelden.

```azurecli
az login
```

Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="update"></a>Aktualisieren

Sie können das Paket mit dem Befehl `zypper update` aktualisieren.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Entfernen Sie das Paket aus Ihrem System.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

