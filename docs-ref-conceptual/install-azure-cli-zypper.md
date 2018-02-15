---
title: Installieren der Azure CLI 2.0 unter Linux mit zypper
description: Installieren der Azure CLI 2.0 mit zypper
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6ee3aff74f43fab0c80c58c7fe57c9fa74a6ef2f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="d5720-103">Installieren der Azure CLI 2.0 mit zypper</span><span class="sxs-lookup"><span data-stu-id="d5720-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="d5720-104">Wenn Sie eine Distribution mit `zypper` verwenden (etwa openSUSE oder SLES), steht ein Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d5720-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="d5720-105">Dieses Paket wurde mit openSUSE 42.2 und SLES 12 SP 2 getestet.</span><span class="sxs-lookup"><span data-stu-id="d5720-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="d5720-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="d5720-106">Install</span></span>

1. <span data-ttu-id="d5720-107">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="d5720-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="d5720-108">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="d5720-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="d5720-109">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="d5720-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="d5720-110">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="d5720-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="d5720-111">Sie können die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="d5720-111">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="d5720-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d5720-112">Update</span></span>

<span data-ttu-id="d5720-113">Sie können das Paket mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d5720-113">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d5720-114">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d5720-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d5720-115">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="d5720-115">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="d5720-116">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="d5720-116">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="d5720-117">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="d5720-117">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

