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
ms.openlocfilehash: 6b9a97e73f45c8271f1e8f19d5a8cf5f9f748d07
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="541ba-104">Installieren der Azure CLI 2.0 mit zypper</span><span class="sxs-lookup"><span data-stu-id="541ba-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="541ba-105">Wenn Sie eine Distribution ausführen, in der `zypper` enthalten ist (etwa OpenSUSE oder SLE), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.</span><span class="sxs-lookup"><span data-stu-id="541ba-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="541ba-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="541ba-106">Install</span></span>

1. <span data-ttu-id="541ba-107">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="541ba-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="541ba-108">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="541ba-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="541ba-109">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="541ba-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="541ba-110">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="541ba-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="541ba-111">Sie können die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="541ba-111">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="541ba-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="541ba-112">Update</span></span>

<span data-ttu-id="541ba-113">Sie können das Paket mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="541ba-113">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="541ba-114">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="541ba-114">Uninstall</span></span>

<span data-ttu-id="541ba-115">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="541ba-115">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="541ba-116">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="541ba-116">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="541ba-117">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="541ba-117">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="541ba-118">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="541ba-118">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="541ba-119">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="541ba-119">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="541ba-120">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="541ba-120">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="541ba-121">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="541ba-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

