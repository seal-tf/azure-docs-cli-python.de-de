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
ms.openlocfilehash: de695454c6f3109679b9eb9f6c0d77348d354518
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="4d57c-104">Installieren der Azure CLI 2.0 mit yum</span><span class="sxs-lookup"><span data-stu-id="4d57c-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="4d57c-105">Wenn Sie eine Distribution ausführen, in der `yum` enthalten ist (etwa RHEL, Fedora oder CentOS), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.</span><span class="sxs-lookup"><span data-stu-id="4d57c-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="4d57c-106">Sie benötigen Python 2.7.x oder Python 3.x, um die CLI nutzen zu können.</span><span class="sxs-lookup"><span data-stu-id="4d57c-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="4d57c-107">[Installieren Sie Python](https://www.python.org/downloads/), wenn Ihre Distribution keines dieser Pakete enthält.</span><span class="sxs-lookup"><span data-stu-id="4d57c-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="4d57c-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="4d57c-108">Install</span></span> 

1. <span data-ttu-id="4d57c-109">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="4d57c-109">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="4d57c-110">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="4d57c-110">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="4d57c-111">Aktualisieren Sie den `yum`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="4d57c-111">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="4d57c-112">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="4d57c-112">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="4d57c-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4d57c-113">Update</span></span>

<span data-ttu-id="4d57c-114">Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.</span><span class="sxs-lookup"><span data-stu-id="4d57c-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="4d57c-115">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="4d57c-115">Uninstall</span></span>

<span data-ttu-id="4d57c-116">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="4d57c-116">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="4d57c-117">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="4d57c-117">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="4d57c-118">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="4d57c-118">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="4d57c-119">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4d57c-119">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="4d57c-120">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="4d57c-120">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="4d57c-121">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="4d57c-121">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="4d57c-122">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="4d57c-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
