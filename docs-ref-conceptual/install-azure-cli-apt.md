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
ms.openlocfilehash: a2578c79ba961cb12f3f49e77a9eaa73c4fe97a2
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="8f12c-103">Installieren der Azure CLI 2.0 mit apt</span><span class="sxs-lookup"><span data-stu-id="8f12c-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="8f12c-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="8f12c-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="8f12c-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="8f12c-105">This package has been tested with:</span></span>

* <span data-ttu-id="8f12c-106">Ubuntu Trusty, Xenial und Artful</span><span class="sxs-lookup"><span data-stu-id="8f12c-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="8f12c-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="8f12c-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="8f12c-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="8f12c-108">Install</span></span>

1. <span data-ttu-id="8f12c-109">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="8f12c-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="8f12c-110">Rufen Sie den Microsoft-Signaturschlüssel ab:</span><span class="sxs-lookup"><span data-stu-id="8f12c-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="8f12c-111">Dieser Signaturschlüssel ist veraltet und wird Ende Mai 2018 ersetzt.</span><span class="sxs-lookup"><span data-stu-id="8f12c-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="8f12c-112">Stellen Sie sicher, dass Sie auch den neuen Schlüssel installieren, um mit `apt` weiterhin Updates zu erhalten:</span><span class="sxs-lookup"><span data-stu-id="8f12c-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="8f12c-113">Installieren Sie die Befehlszeilenschnittstelle:</span><span class="sxs-lookup"><span data-stu-id="8f12c-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="8f12c-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="8f12c-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="8f12c-115">Führen Sie den Befehl `az login` aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="8f12c-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="8f12c-116">Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8f12c-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="8f12c-117">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="8f12c-117">Troubleshooting</span></span>

<span data-ttu-id="8f12c-118">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="8f12c-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="8f12c-119">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8f12c-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="8f12c-120">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="8f12c-120">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="8f12c-121">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="8f12c-121">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="8f12c-122">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="8f12c-122">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="8f12c-123">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="8f12c-123">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="8f12c-124">Keine Reaktion von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="8f12c-124">apt-key hangs</span></span>

<span data-ttu-id="8f12c-125">Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="8f12c-125">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="8f12c-126">Für Ihre Firewall muss möglicherweise ein HTTP-Proxy für ausgehende Verbindungen verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="8f12c-126">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="8f12c-127">Wenn Sie nicht wissen, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator.</span><span class="sxs-lookup"><span data-stu-id="8f12c-127">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="8f12c-128">Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer, Kennwort und `@`-Token weg.</span><span class="sxs-lookup"><span data-stu-id="8f12c-128">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="8f12c-129">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8f12c-129">Update</span></span>

<span data-ttu-id="8f12c-130">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="8f12c-130">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="8f12c-131">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="8f12c-131">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="8f12c-132">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="8f12c-132">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="8f12c-133">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="8f12c-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="8f12c-134">Deinstallieren Sie sie mit `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="8f12c-134">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="8f12c-135">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="8f12c-135">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="8f12c-136">Entfernen Sie alle nicht benötigten Pakete.</span><span class="sxs-lookup"><span data-stu-id="8f12c-136">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
