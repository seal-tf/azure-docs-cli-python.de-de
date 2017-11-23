---
title: Azure CLI 2.0-Erweiterungen
description: Verwenden von Erweiterungen mit Azure CLI 2.0
keywords: Azure CLI, Erweiterungen
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 930073324d68f9719ce5035388120e7b6ac41a98
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/18/2017
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Verwenden von Erweiterungen mit Azure CLI 2.0

Erweiterungen sind einzelne Module, die nicht mit der Azure CLI bereitgestellt werden und die Ihnen das Hinzufügen von Funktionen mit neuen Befehlen ermöglichen. Dies können experimentelle oder Vorabangebote, spezielle Tools, die Microsoft zur Erfüllung Ihrer Anforderungen bereitstellt, oder auch von Ihnen selbst geschriebene Erweiterungen sein. Erweiterungen ermöglichen das flexible Anpassen der CLI an Ihre eigenen Anforderungen, ohne dass Sie viele zusätzliche Pakete mitliefern müssen, die nicht als Teil des Kernfeaturesatzes angesehen werden.

In diesem Artikel wird beschrieben, wie Sie Erweiterungen für die CLI installieren, aktualisieren und entfernen. Außerdem werden häufige Fragen zum Verhalten von Erweiterungen beantwortet.

## <a name="finding-extensions"></a>Suchen nach Erweiterungen

Um zu ermitteln, welche Erweiterungen verfügbar sind, können Sie `az extension list-available` verwenden. Mit diesem Befehl werden die verfügbaren offiziellen Erweiterungen aufgelistet, die von Microsoft bereitgestellt und unterstützt werden.

## <a name="installing-extensions"></a>Installieren von Erweiterungen

Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie `az extension add` verwenden, um sie abzurufen. Wenn die Erweiterung eine offizielle Microsoft-Erweiterung ist, die bei Ausführung von `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.

```azurecli
az extension add --name <extension-name>
```

Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, können Sie die Quell-URL oder den lokalen Pfad angeben. Dies _muss_ eine kompilierte Python-Wheeldatei sein.

```azurecli
az extension add --source <URL-or-path>
```

Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`. Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).

## <a name="updating-extensions"></a>Aktualisieren von Erweiterungen

Erweiterungen können nur anhand des Namens aktualisiert werden:

```azurecli
az extension update --name <extension-name>
```

Wenn ein Erweiterungsname aus einem bestimmten Grund für die CLI nicht aufgelöst werden kann, sollten Sie die Erweiterung neu installieren, um sie zu aktualisieren. Außerdem ist es möglich, dass die Erweiterung nicht mehr als Vorschauversion verfügbar und zu einem integrierten Befehl für die CLI geworden ist. Aktualisieren Sie in diesem Fall die CLI, und deinstallieren Sie die Erweiterung.

## <a name="uninstalling-extensions"></a>Deinstallieren von Erweiterungen

Wenn Sie eine Erweiterung nicht mehr benötigen, können Sie sie mit `az extension remove` entfernen.

```azurecli
az extension remove --name <extension-name>
```

Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen. Dies ist der Wert der Shellvariablen `$AZURE_EXTENSION_DIR`. Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

Es wird empfohlen, die Deinstallation mit `az extension remove` durchzuführen.

## <a name="faq"></a>Häufig gestellte Fragen

Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.

### <a name="what-file-formats-are-allowed-for-installation"></a>Welche Dateiformate sind für die Installation zulässig?

Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.

### <a name="can-extensions-replace-existing-commands"></a>Können Erweiterungen vorhandene Befehle ersetzen?

Ja. Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?

Für eine Erweiterung sollte in der dazugehörigen Dokumentation und in den Versionsinformationen angegeben sein, wenn es sich um eine Vorabversion handelt. Es kommt auch häufiger vor, dass Microsoft Vorschauversionen von Befehlen für die CLI als Erweiterungen veröffentlicht, die nach der Vorschauphase des Produkts in die Hauptoberfläche der CLI integriert werden sollen.

### <a name="can-extensions-depend-upon-each-other"></a>Können Erweiterungen voneinander abhängig sein?

Nein. Erweiterungen müssen einzelne Pakete sein, die nicht voneinander abhängig sind. Dies liegt daran, dass für die CLI nicht garantiert ist, wann Erweiterungen geladen werden. Es kann also nicht sichergestellt werden, dass die Anforderungen von Abhängigkeiten erfüllt werden. Bei der Installation einer Erweiterung wird nur die jeweilige Erweiterung installiert, und sie sollte auch dann funktionieren, wenn Sie andere Erweiterungen entfernen.

### <a name="are-extensions-updated-along-with-the-cli"></a>Werden Erweiterungen zusammen mit der CLI aktualisiert?

Nein. Erweiterungen müssen separat aktualisiert werden, wie im Abschnitt [Aktualisieren von Erweiterungen](#updating-extensions) beschrieben.
