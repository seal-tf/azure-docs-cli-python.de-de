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
ms.openlocfilehash: 4076fefb902a324f77f97bc042b9f5ba3e787734
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="cda30-103">Installieren der Azure CLI 2.0 mit apt</span><span class="sxs-lookup"><span data-stu-id="cda30-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="cda30-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="cda30-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="cda30-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="cda30-105">This package has been tested with:</span></span>

* <span data-ttu-id="cda30-106">Ubuntu Wheezy, Xenial und Artful</span><span class="sxs-lookup"><span data-stu-id="cda30-106">Ubuntu wheezy, xenial, and artful</span></span>
* <span data-ttu-id="cda30-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="cda30-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="cda30-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="cda30-108">Install</span></span>

1. <span data-ttu-id="cda30-109">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="cda30-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="cda30-110">Führen Sie die folgenden sudo-Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="cda30-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="cda30-111">Sie können die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="cda30-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="cda30-112">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="cda30-112">Troubleshooting</span></span>

<span data-ttu-id="cda30-113">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="cda30-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="cda30-114">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="cda30-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="cda30-115">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="cda30-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="cda30-116">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="cda30-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="cda30-117">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda30-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="cda30-118">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="cda30-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="cda30-119">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cda30-119">Update</span></span>

<span data-ttu-id="cda30-120">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="cda30-120">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="cda30-121">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="cda30-121">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="cda30-122">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="cda30-122">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="cda30-123">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="cda30-123">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="cda30-124">Deinstallieren Sie sie mit `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="cda30-124">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="cda30-125">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="cda30-125">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="cda30-126">Entfernen Sie alle nicht benötigten Pakete.</span><span class="sxs-lookup"><span data-stu-id="cda30-126">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
