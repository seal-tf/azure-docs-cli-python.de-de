---
title: Abfragen von Befehlsergebnissen mit Azure CLI 2.0
description: "Erfahren Sie, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI 2.0-Befehlen ausführen."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98bc35c1e8136231011a2303901f42c68c9a7758
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="b92c6-103">Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="b92c6-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="b92c6-104">Für Azure CLI 2.0 wird der Parameter `--query` verwendet, um eine [JMESPath-Abfrage](http://jmespath.org) zu den Ergebnissen Ihres `az`-Befehls durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="b92c6-104">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="b92c6-105">JMESPath ist eine leistungsstarke Sprache für JSON-Ausgaben.</span><span class="sxs-lookup"><span data-stu-id="b92c6-105">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="b92c6-106">Wenn Sie mit JMESPath-Abfragen nicht vertraut sein sollten, ist das Tutorial unter [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html) hilfreich.</span><span class="sxs-lookup"><span data-stu-id="b92c6-106">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="b92c6-107">Der Parameter `Query` wird von jedem Ressourcentyp (Container Services, Web-Apps, VM usw.) in Azure CLI 2.0 unterstützt und kann für verschiedene Zwecke verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b92c6-107">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="b92c6-108">Hier sind einige Beispiele aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="b92c6-108">We have listed several examples below.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="b92c6-109">Auswählen einfacher Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b92c6-109">Select simple properties</span></span>

<span data-ttu-id="b92c6-110">Der einfache Befehl `list` mit dem Ausgabeformat `table` gibt einen fertigen Satz mit den gängigsten einfachen Eigenschaften für jeden Ressourcentyp in einem leicht lesbaren Tabellenformat zurück.</span><span class="sxs-lookup"><span data-stu-id="b92c6-110">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

<span data-ttu-id="b92c6-111">Sie können den Parameter `--query` verwenden, um nur den Ressourcengruppennamen und VM-Namen für alle virtuellen Computer Ihres Abonnements anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="b92c6-111">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query "[].[name, resourceGroup]" --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

<span data-ttu-id="b92c6-112">Im vorherigen Beispiel lauten die Spaltenüberschriften „Column1“ und „Column2“.</span><span class="sxs-lookup"><span data-stu-id="b92c6-112">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="b92c6-113">Außerdem können Sie den Eigenschaften auch benutzerfreundliche Bezeichnungen und Namen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b92c6-113">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="b92c6-114">Im folgenden Beispiel haben wir den ausgewählten Eigenschaften „name“ und „resourceGroup“ die Bezeichnungen „VMName“ und „RGName“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b92c6-114">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="b92c6-115">Auswählen komplexer geschachtelter Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b92c6-115">Select complex nested properties</span></span>

<span data-ttu-id="b92c6-116">Wenn sich die Eigenschaft, die Sie auswählen möchten, tief in der Struktur der JSON-Ausgabe befindet, müssen Sie den vollständigen Pfad zu dieser geschachtelten Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="b92c6-116">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="b92c6-117">Das folgende Beispiel zeigt, wie Sie den VM-Namen und den Betriebssystemtyp über den Befehl „vm list“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="b92c6-117">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="b92c6-118">Filtern mit der Funktion „contains“</span><span class="sxs-lookup"><span data-stu-id="b92c6-118">Filter with the contains function</span></span>

<span data-ttu-id="b92c6-119">Sie können die JMESPath-Funktion `contains` verwenden, um die für die Abfrage zurückgegebenen Ergebnisse zu verfeinern.</span><span class="sxs-lookup"><span data-stu-id="b92c6-119">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="b92c6-120">Im folgenden Beispiel wählt der Befehl nur virtuelle Computer aus, deren Name „RGD“ enthält.</span><span class="sxs-lookup"><span data-stu-id="b92c6-120">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

<span data-ttu-id="b92c6-121">Im nächsten Beispiel werden die virtuellen Computer zurückgegeben, bei denen „vmSize“ den Wert „Standard_DS1“ hat.</span><span class="sxs-lookup"><span data-stu-id="b92c6-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a><span data-ttu-id="b92c6-122">Filtern mit grep</span><span class="sxs-lookup"><span data-stu-id="b92c6-122">Filter with grep</span></span>

<span data-ttu-id="b92c6-123">Für das Ausgabeformat `tsv` wird Text mit Tabulatortrennung und ohne Überschriften erzeugt.</span><span class="sxs-lookup"><span data-stu-id="b92c6-123">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="b92c6-124">Es kann per Pipe-Zeichen an Befehle wie `grep` und `cut` angefügt werden, um bestimmte Werte der Ausgabe von `list` weiter zu analysieren.</span><span class="sxs-lookup"><span data-stu-id="b92c6-124">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="b92c6-125">Im folgenden Beispiel werden mit dem Befehl `grep` nur virtuelle Computer ausgewählt, deren Name „RGD“ enthält.</span><span class="sxs-lookup"><span data-stu-id="b92c6-125">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="b92c6-126">Mit dem Befehl `cut` wird nur der Wert des achten Felds (durch Tabulatoren getrennt) für die Anzeige in der Ausgabe ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b92c6-126">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="b92c6-127">Durchführen einer Untersuchung mit jpterm</span><span class="sxs-lookup"><span data-stu-id="b92c6-127">Explore with jpterm</span></span>

<span data-ttu-id="b92c6-128">Sie können die Befehlsausgabe auch per Pipe-Zeichen an [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) anfügen und mit Ihrer JMESPath-Abfrage experimentieren.</span><span class="sxs-lookup"><span data-stu-id="b92c6-128">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

