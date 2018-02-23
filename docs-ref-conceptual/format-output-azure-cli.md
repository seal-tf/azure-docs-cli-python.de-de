---
title: "Ausgabeformate für Azure CLI 2.0"
description: Erfahren Sie, wie Sie die Ausgabe von Azure CLI 2.0-Befehlen in Tabellen, Listen oder JSON-Code formatieren.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a5d629675b468421e3abee41b9c8bffd7e96e5b0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Ausgabeformate für Azure CLI 2.0-Befehle

Für Azure CLI 2.0 wird JSON als Standardoption für die Ausgabe verwendet, aber Sie haben verschiedene Möglichkeiten, die Ausgabe von Befehlen zu formatieren.  Verwenden Sie den Parameter `--output` (oder `--out` oder `-o`), um die Ausgabe des Befehls basierend auf einem der Ausgabetypen zu formatieren, die in der folgenden Tabelle angegeben sind.

--output | BESCHREIBUNG
---------|-------------------------------
`json`   | JSON-Zeichenfolge. `json` ist die Standardeinstellung.
`jsonc`  | Farbige JSON-Zeichenfolge
`table`  | Tabelle mit Spaltenüberschriften
`tsv`    | Per Tabulator getrennte Werte

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a>Verwenden der Option „json“

Im folgenden Beispiel wird die Liste mit den virtuellen Computern Ihrer Abonnements im JSON-Standardformat angezeigt.

```azurecli-interactive
az vm list --output json
```

Die Ergebnisse werden wie folgt angezeigt (aus Platzgründen nur eine Teilausgabe).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="using-the-table-option"></a>Verwenden der Option „table“

Mit der Option „table“ wird eine leicht lesbare Ausgabe bereitgestellt. Beachten Sie aber, dass geschachtelte Objekte beim einfachen Befehl `--output table` nicht in die Ausgabe einbezogen werden (im Gegensatz zum obigen json-Beispiel).  Bei Verwendung des gleichen Beispiels mit dem Ausgabeformat „table“ wird eine Liste mit den ausgewählten häufigsten Eigenschaftswerten bereitgestellt.

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

Sie können den Parameter `--query` verwenden, um die Eigenschaften und Spalten anzupassen, die Sie in der Listenausgabe anzeigen möchten. Im folgenden Beispiel wird veranschaulicht, wie Sie im Befehl `list` nur den VM-Namen und den Ressourcengruppennamen auswählen.

```azurecli-interactive
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a>Verwenden der Option „tsv“

Beim Ausgabeformat „tsv“ wird eine einfache textbasierte und per Tabulator getrennte Ausgabe ohne Überschriften und Bindestriche zurückgegeben. Mit diesem Format ist es leicht, die Ausgabe in anderen Befehlen und Tools zu nutzen, in denen der Text verarbeitet werden muss. Wenn das obige Beispiel mit der Option `tsv` verwendet wird, wird das Ergebnis mit Tabulatortrennung ausgegeben.

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

Im nächsten Beispiel wird veranschaulicht, wie Sie die Ausgabe von `tsv` per Pipe-Zeichen an Befehle wie `grep` und `cut` anfügen können, um bestimmte Werte der Ausgabe von `list` weiter zu analysieren. Mit dem Befehl `grep` werden nur Elemente ausgewählt, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` nur der Wert des achten Felds (getrennt durch Tabulatoren) für die Anzeige in der Ausgabe ausgewählt.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>Festlegen des Standardformats für die Ausgabe

Sie können den Befehl `az configure` verwenden, um Ihre Umgebung einzurichten oder die bevorzugten Einstellungen festzulegen, z.B. Standardeinstellungen für Ausgabeformate. Die einfachste Standardeinstellung für das Ausgabeformat zur normalen Nutzung ist das Format „table“. Wählen Sie die Option **3**, wenn Sie zum Angeben des Ausgabeformats aufgefordert werden.

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]:
```
