---
title: Abfragen von Befehlsergebnissen mit Azure CLI 2.0
description: "Verwenden Sie „--query“ zum Durchführen von JMESPath-Abfragen für die Ausgabe von Azure CLI 2.0-Befehlen."
keywords: Azure CLI 2.0, JMESPath, Abfrage, Linux, MacOS, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: 23c743210ccc506935f6e78489ca0df2b99d46a1
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a>Verwenden von JMESPath-Abfragen mit Azure CLI 2.0

Für Azure CLI 2.0 wird der Parameter `--query` verwendet, um eine [JMESPath-Abfrage](http://jmespath.org) zu den Ergebnissen Ihres `az`-Befehls durchzuführen. JMESPath ist eine leistungsstarke Sprache für JSON-Ausgaben.  Wenn Sie mit JMESPath-Abfragen nicht vertraut sein sollten, ist das Tutorial unter [JMESPath.org/tutorial](http:/JMESPath.org/tutorial.html) hilfreich.

Der Parameter `Query` wird von jedem Ressourcentyp (Container Services, Web-Apps, VM usw.) in Azure CLI 2.0 unterstützt und kann für verschiedene Zwecke verwendet werden.  Hier sind einige Beispiele aufgeführt.

## <a name="selecting-simple-properties"></a>Auswählen einfacher Eigenschaften

Der einfache Befehl `list` mit dem Ausgabeformat `table` gibt einen fertigen Satz mit den gängigsten einfachen Eigenschaften für jeden Ressourcentyp in einem leicht lesbaren Tabellenformat zurück.

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

Sie können den Parameter `--query` verwenden, um nur den Ressourcengruppennamen und VM-Namen für alle virtuellen Computer Ihres Abonnements anzuzeigen.

```azurecli-interactive
az vm list \
  --query [*].[name,resourceGroup] --out table
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

Im vorherigen Beispiel lauten die Spaltenüberschriften „Column1“ und „Column2“.  Außerdem können Sie den Eigenschaften auch benutzerfreundliche Bezeichnungen und Namen hinzufügen.  Im folgenden Beispiel haben wir den ausgewählten Eigenschaften „name“ und „resourceGroup“ die Bezeichnungen „VMName“ und „RGName“ hinzugefügt.


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

## <a name="selecting-complex-nested-properties"></a>Auswählen komplexer geschachtelter Eigenschaften

Wenn sich die Eigenschaft, die Sie auswählen möchten, tief in der Struktur der JSON-Ausgabe befindet, müssen Sie den vollständigen Pfad zu dieser geschachtelten Eigenschaft angeben. Das folgende Beispiel zeigt, wie Sie den VM-Namen und den Betriebssystemtyp über den Befehl „vm list“ auswählen.

```azurecli-interactive
az vm list \
  --query "[].{VMName:name,OSType:storageProfile.osDisk.osType}" --out table
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

## <a name="filter-with-the-contains-function"></a>Filtern mit der Funktion „contains“

Sie können die JMESPath-Funktion `contains` verwenden, um die für die Abfrage zurückgegebenen Ergebnisse zu verfeinern.
Im folgenden Beispiel wählt der Befehl nur virtuelle Computer aus, deren Name „RGD“ enthält.  

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup,'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

Im nächsten Beispiel werden die virtuellen Computer zurückgegeben, bei denen „vmSize“ den Wert „Standard_DS1“ hat.

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

## <a name="filter-with-grep"></a>Filtern mit grep

Für das Ausgabeformat `tsv` wird Text mit Tabulatortrennung und ohne Überschriften erzeugt. Es kann per Pipe-Zeichen an Befehle wie `grep` und `cut` angefügt werden, um bestimmte Werte der Ausgabe von `list` weiter zu analysieren. Im folgenden Beispiel werden mit dem Befehl `grep` nur virtuelle Computer ausgewählt, deren Name „RGD“ enthält.  Mit dem Befehl `cut` wird nur der Wert des achten Felds (durch Tabulatoren getrennt) für die Anzeige in der Ausgabe ausgewählt.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Durchführen einer Untersuchung mit jpterm

Sie können die Befehlsausgabe auch per Pipe-Zeichen an [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) anfügen und mit Ihrer JMESPath-Abfrage experimentieren.

```bash
pip install jmespath-terminal
az vm list | jpterm
```

