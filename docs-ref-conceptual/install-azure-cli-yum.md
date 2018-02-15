---
title: Installieren der Azure CLI 2.0 unter Linux mit yum
description: Installieren der Azure CLI 2.0 mit yum
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4b92499d2cb81f64bfbb13215428365711b07874
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="b3ff2-103">Installieren der Azure CLI 2.0 mit yum</span><span class="sxs-lookup"><span data-stu-id="b3ff2-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="b3ff2-104">Wenn Sie eine Distribution mit `yum` verwenden (etwa RHEL, Fedora oder CentOS), steht ein Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="b3ff2-105">Dieses Paket wurde mit RHEL 7, Fedora 19 (und höher) und CentOS 7 getestet.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="b3ff2-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="b3ff2-106">Install</span></span>

1. <span data-ttu-id="b3ff2-107">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="b3ff2-107">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="b3ff2-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="b3ff2-108">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="b3ff2-109">Aktualisieren Sie den `yum`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="b3ff2-109">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="b3ff2-110">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-110">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="b3ff2-111">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b3ff2-111">Update</span></span>

<span data-ttu-id="b3ff2-112">Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-112">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="b3ff2-113">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="b3ff2-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b3ff2-114">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-114">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="b3ff2-115">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-115">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="b3ff2-116">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="b3ff2-116">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
