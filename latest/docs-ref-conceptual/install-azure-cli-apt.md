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
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="3d7ac-104">Installieren der Azure CLI 2.0 mit apt</span><span class="sxs-lookup"><span data-stu-id="3d7ac-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="3d7ac-105">Wenn Sie eine Distribution ausführen, in der `apt` enthalten ist (etwa Ubuntu oder Debian), steht ein Paket für die Azure CLI zur Verfügung, das Sie auf Ihrem System installieren können.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="3d7ac-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="3d7ac-106">Install</span></span>

1. <span data-ttu-id="3d7ac-107">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="3d7ac-107">Modify your sources list:</span></span>

   - <span data-ttu-id="3d7ac-108">32-Bit-System</span><span class="sxs-lookup"><span data-stu-id="3d7ac-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="3d7ac-109">64-Bit-System</span><span class="sxs-lookup"><span data-stu-id="3d7ac-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="3d7ac-110">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="3d7ac-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="3d7ac-111">Sie können die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="3d7ac-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3d7ac-112">Update</span></span>

<span data-ttu-id="3d7ac-113">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-113">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="3d7ac-114">Dadurch werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-114">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="3d7ac-115">Um nur die CLI zu aktualisieren, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-115">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="3d7ac-116">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="3d7ac-116">Uninstall</span></span>

<span data-ttu-id="3d7ac-117">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="3d7ac-118">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="3d7ac-119">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="3d7ac-120">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3d7ac-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="3d7ac-121">Deinstallieren Sie sie mit `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-121">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="3d7ac-122">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-122">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="3d7ac-123">Entfernen Sie alle nicht benötigten Pakete.</span><span class="sxs-lookup"><span data-stu-id="3d7ac-123">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
