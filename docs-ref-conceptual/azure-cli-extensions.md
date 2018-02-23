---
title: Azure CLI 2.0-Erweiterungen
description: Verwenden von Erweiterungen mit Azure CLI 2.0
keywords: Azure CLI, Erweiterungen
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 548c06c64cc98598a2bd24bcc5959e59bffb4930
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="ebaf0-104">Verwenden von Erweiterungen mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ebaf0-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="ebaf0-105">Erweiterungen sind einzelne Module, die nicht mit der Azure CLI bereitgestellt werden und Funktionen über neue Befehle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="ebaf0-106">Dies können experimentelle Angebote oder Vorabangebote, spezielle Tools von Microsoft oder von Ihnen selbst geschriebene benutzerdefinierte Features sein.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="ebaf0-107">Erweiterungen ermöglichen das flexible Anpassen der CLI an Ihre eigenen Anforderungen, ohne dass Sie viele zusätzliche Pakete mitliefern müssen, die nicht als Teil des Kernfeaturesatzes angesehen werden.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="ebaf0-108">In diesem Artikel wird beschrieben, wie Sie Erweiterungen für die CLI installieren, aktualisieren und entfernen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="ebaf0-109">Außerdem werden häufige Fragen zum Verhalten von Erweiterungen beantwortet.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="ebaf0-110">Suchen nach Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ebaf0-110">Finding extensions</span></span>

<span data-ttu-id="ebaf0-111">Um zu ermitteln, welche Erweiterungen verfügbar sind, können Sie [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available) verwenden.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available).</span></span> <span data-ttu-id="ebaf0-112">Mit diesem Befehl werden die verfügbaren offiziellen Erweiterungen aufgelistet, die von Microsoft bereitgestellt und unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="ebaf0-113">Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ebaf0-113">Installing extensions</span></span>

<span data-ttu-id="ebaf0-114">Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) verwenden, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-114">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) to get it.</span></span> <span data-ttu-id="ebaf0-115">Wenn die Erweiterung in `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-115">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="ebaf0-116">Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, können Sie die Quell-URL oder den lokalen Pfad angeben.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="ebaf0-117">Dies _muss_ eine kompilierte Python-Wheeldatei sein.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="ebaf0-118">Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="ebaf0-119">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="ebaf0-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="ebaf0-120">Aktualisieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ebaf0-120">Updating extensions</span></span>

<span data-ttu-id="ebaf0-121">Erweiterungen können nur anhand des Namens aktualisiert werden (mit [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update)).</span><span class="sxs-lookup"><span data-stu-id="ebaf0-121">Extensions can only be updated by name, using [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="ebaf0-122">Wenn ein Erweiterungsname aus einem bestimmten Grund für die CLI nicht aufgelöst werden kann, sollten Sie die Erweiterung neu installieren, um sie zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="ebaf0-123">Außerdem ist es möglich, dass die Erweiterung nicht mehr als Vorschauversion verfügbar und zu einem integrierten Befehl für die CLI geworden ist.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="ebaf0-124">Aktualisieren Sie in diesem Fall die CLI, und deinstallieren Sie die Erweiterung.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="ebaf0-125">Deinstallieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ebaf0-125">Uninstalling extensions</span></span>

<span data-ttu-id="ebaf0-126">Wenn Sie eine Erweiterung nicht mehr benötigen, können Sie sie mit [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove) entfernen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-126">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="ebaf0-127">Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="ebaf0-128">Dies ist der Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="ebaf0-129">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="ebaf0-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="ebaf0-130">Es wird empfohlen, die Deinstallation mit `az extension remove` durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="ebaf0-131">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="ebaf0-131">FAQ</span></span>

<span data-ttu-id="ebaf0-132">Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="ebaf0-133">Welche Dateiformate sind für die Installation zulässig?</span><span class="sxs-lookup"><span data-stu-id="ebaf0-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="ebaf0-134">Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="ebaf0-135">Können Erweiterungen vorhandene Befehle ersetzen?</span><span class="sxs-lookup"><span data-stu-id="ebaf0-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="ebaf0-136">Ja.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-136">Yes.</span></span> <span data-ttu-id="ebaf0-137">Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="ebaf0-138">Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?</span><span class="sxs-lookup"><span data-stu-id="ebaf0-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="ebaf0-139">Für eine Erweiterung sollte in der dazugehörigen Dokumentation und in den Versionsinformationen angegeben sein, wenn es sich um eine Vorabversion handelt.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="ebaf0-140">Es kommt auch häufiger vor, dass Microsoft Vorschauversionen von Befehlen für die CLI als Erweiterungen veröffentlicht, die nach der Vorschauphase des Produkts in die Hauptoberfläche der CLI integriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="ebaf0-141">Können Erweiterungen voneinander abhängig sein?</span><span class="sxs-lookup"><span data-stu-id="ebaf0-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="ebaf0-142">Nein.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-142">No.</span></span> <span data-ttu-id="ebaf0-143">Erweiterungen müssen einzelne Pakete sein, die nicht voneinander abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="ebaf0-144">Dies liegt daran, dass für die CLI nicht garantiert ist, wann Erweiterungen geladen werden. Es kann also nicht sichergestellt werden, dass die Anforderungen von Abhängigkeiten erfüllt werden.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="ebaf0-145">Bei der Installation einer Erweiterung wird nur die jeweilige Erweiterung installiert, und sie sollte auch dann funktionieren, wenn Sie andere Erweiterungen entfernen.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="ebaf0-146">Werden Erweiterungen zusammen mit der CLI aktualisiert?</span><span class="sxs-lookup"><span data-stu-id="ebaf0-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="ebaf0-147">Nein.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-147">No.</span></span> <span data-ttu-id="ebaf0-148">Erweiterungen müssen separat aktualisiert werden, wie im Abschnitt [Aktualisieren von Erweiterungen](#updating-extensions) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="ebaf0-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>
