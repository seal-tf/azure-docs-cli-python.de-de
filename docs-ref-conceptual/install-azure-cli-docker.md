---
title: Installieren der Azure CLI mit Docker
description: Installieren eines Docker-Containers mit der Azure CLI 2.0
keywords: Azure CLI,Azure CLI installieren,Azure Docker,Azure Docker-Image,
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 7a12da712cd2aad5bb5fb56e27267a8e05df34a6
ms.sourcegitcommit: c95a0cde5819cfe8a4f6b058a52f09a8f87c9696
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2018
---
# <a name="install-azure-cli-20-with-docker"></a><span data-ttu-id="df948-104">Installieren der Azure CLI 2.0 mit Docker</span><span class="sxs-lookup"><span data-stu-id="df948-104">Install Azure CLI 2.0 with Docker</span></span>

<span data-ttu-id="df948-105">Sie können Docker zum Installieren eines eigenständigen Linux-Containers mit der vorinstallierten Azure CLI 2.0 verwenden.</span><span class="sxs-lookup"><span data-stu-id="df948-105">You can use Docker to install a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="df948-106">Dies ermöglicht einen schnellen Einstieg in eine Umgebung, in der Sie die CLI ausprobieren und somit testen können, ob sie für Sie geeignet ist. Eine Verwendung als Basisimage ist ebenfalls möglich.</span><span class="sxs-lookup"><span data-stu-id="df948-106">This lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or allows you to use this as a base image.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="df948-107">Installieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="df948-107">Install with Docker</span></span>

<span data-ttu-id="df948-108">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="df948-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli:<version>
   ```

<span data-ttu-id="df948-109">Verfügbare Versionen finden Sie in unseren [Docker-Tags](https://hub.docker.com/r/microsoft/azure-cli/tags/).</span><span class="sxs-lookup"><span data-stu-id="df948-109">See our [Docker tags](https://hub.docker.com/r/microsoft/azure-cli/tags/) for available versions.</span></span>

<span data-ttu-id="df948-110">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="df948-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="df948-111">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="df948-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli:<version>
> ```

### <a name="update-with-docker"></a><span data-ttu-id="df948-112">Aktualisieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="df948-112">Update with Docker</span></span>

<span data-ttu-id="df948-113">Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df948-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="df948-114">Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.</span><span class="sxs-lookup"><span data-stu-id="df948-114">For this reason you should try and avoid using a container which hosts the CLI as a data store.</span></span>

1. <span data-ttu-id="df948-115">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="df948-115">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull microsoft/azure-cli
   ```

2. <span data-ttu-id="df948-116">Rufen Sie die Container ab, die derzeit das CLI-Image verwenden.</span><span class="sxs-lookup"><span data-stu-id="df948-116">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > <span data-ttu-id="df948-117">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="df948-117">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="df948-118">Halten Sie die Container an, und erstellen Sie sie neu.</span><span class="sxs-lookup"><span data-stu-id="df948-118">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run microsoft/azure-cli
   ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="df948-119">Deinstallieren mit Docker</span><span class="sxs-lookup"><span data-stu-id="df948-119">Uninstall with Docker</span></span>

<span data-ttu-id="df948-120">Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="df948-120">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="df948-121">Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können.</span><span class="sxs-lookup"><span data-stu-id="df948-121">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="df948-122">Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist.</span><span class="sxs-lookup"><span data-stu-id="df948-122">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="df948-123">Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="df948-123">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="df948-124">Um das CLI-Docker-Image ordnungsgemäß zu deinstallieren, müssen Sie alle Container mit diesem Image entfernen und dann das lokale Image löschen.</span><span class="sxs-lookup"><span data-stu-id="df948-124">To properly uninstall the CLI Docker image you need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="df948-125">Rufen Sie die Container ab, die das azure-cli-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="df948-125">Get the containers running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > <span data-ttu-id="df948-126">Wenn Sie eine bestimmte Version des Images installiert haben, müssen Sie `:<version>` ans Ende des Imagenamens anfügen.</span><span class="sxs-lookup"><span data-stu-id="df948-126">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

2. <span data-ttu-id="df948-127">Löschen Sie alle Container mit dem CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="df948-127">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="df948-128">Entfernen Sie das lokal installierte CLI-Image.</span><span class="sxs-lookup"><span data-stu-id="df948-128">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi microsoft/azure-cli
   ```

