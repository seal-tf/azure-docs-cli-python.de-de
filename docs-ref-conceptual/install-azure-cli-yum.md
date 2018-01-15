---
title: Installieren der Azure CLI 2.0 mit yum
description: Installieren der Azure CLI 2.0 mit yum
keywords: Azure CLI,Azure CLI installieren,Azure yum,Azure RHEL, Azure Fedora, Azure CentOS
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
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-yum"></a>Installieren der Azure CLI 2.0 mit yum

Wenn Sie eine Distribution ausführen, in der `yum` enthalten ist (etwa RHEL, Fedora oder CentOS), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installieren

1. Importieren Sie den Microsoft-Repositoryschlüssel:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Erstellen Sie lokale `azure-cli`-Repositoryinformationen:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Aktualisieren Sie den `yum`-Paketindex, und führen Sie die Installation durch:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

Führen Sie die Azure CLI mit dem Befehl `az` aus.

## <a name="update"></a>Aktualisieren

Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten. Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können. Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist. Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).

1. Entfernen Sie das Paket aus Ihrem System.

   ```bash
   sudo yum remove azure-cli
   ```

2. Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
