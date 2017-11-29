---
title: Installieren der Azure CLI 2.0 mit zypper
description: Installieren der Azure CLI 2.0 mit zypper
keywords: Azure CLI, Azure CLI installieren, Azure CLI zypper, Azure CLI OpenSUSE, Azure CLI SLE
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
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="006ef-104">Installieren der Azure CLI 2.0 mit zypper</span><span class="sxs-lookup"><span data-stu-id="006ef-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="006ef-105">Wenn Sie eine Distribution ausführen, in der `zypper` enthalten ist (etwa OpenSUSE oder SLE), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.</span><span class="sxs-lookup"><span data-stu-id="006ef-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="006ef-106">Sie benötigen Python 2.7.x oder Python 3.x, um die CLI nutzen zu können.</span><span class="sxs-lookup"><span data-stu-id="006ef-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="006ef-107">[Installieren Sie Python](https://www.python.org/downloads/), wenn Ihre Distribution keines dieser Pakete enthält.</span><span class="sxs-lookup"><span data-stu-id="006ef-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="006ef-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="006ef-108">Install</span></span> 

1. <span data-ttu-id="006ef-109">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="006ef-109">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="006ef-110">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="006ef-110">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="006ef-111">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="006ef-111">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="006ef-112">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="006ef-112">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="006ef-113">Sie können die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="006ef-113">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="006ef-114">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="006ef-114">Update</span></span>

<span data-ttu-id="006ef-115">Sie können das Paket mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="006ef-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="006ef-116">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="006ef-116">Uninstall</span></span>

<span data-ttu-id="006ef-117">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="006ef-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="006ef-118">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="006ef-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="006ef-119">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="006ef-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="006ef-120">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="006ef-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="006ef-121">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="006ef-121">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="006ef-122">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="006ef-122">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="006ef-123">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="006ef-123">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

