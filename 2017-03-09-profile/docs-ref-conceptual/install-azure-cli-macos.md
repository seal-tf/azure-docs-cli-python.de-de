---
title: "Installieren der Azure-Befehlszeilenschnittstelle für macOS"
description: Installieren der Azure CLI 2.0 unter macOS
keywords: Azure CLI,Azure CLI installieren,Azure macOS, Azure installieren macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a>Installieren der Azure CLI 2.0 unter macOS

Bei einer macOS-Plattform können Sie die Azure CLI entweder über den [Homebrew-Paket-Manager](http://brew.sh) oder manuell installieren. Die bevorzugte Methode ist Homebrew. Damit werden das Installieren, das Abrufen von Updates und das Deinstallieren vereinfacht.

## <a name="use-homebrew-to-install"></a>Installieren mit Homebrew

Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation. Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren. Es ähnelt anderen Paket-Managern wie `apt` oder `yum`.
Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.

### <a name="install-with-homebrew"></a>Installieren mit Homebrew

Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:

```bash
brew update && brew install azure-cli
```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen.

### <a name="update-with-homebrew"></a>Aktualisieren mit Homebrew

Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert. Ein neues Release ist ungefähr alle zwei Wochen verfügbar. Sie müssen die lokalen Repositoryinformationen und anschließend das CLI-Paket aktualisieren.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>Problembehandlung

Ist beim Installieren oder Aktualisieren der CLI mit Homebrew ein Fehler aufgetreten? Hier sind einige allgemeine Fehler sowie Ansätze zum Diagnostizieren und Beheben der Probleme aufgeführt.

#### <a name="unable-to-find-python-or-installed-packages"></a>Python und installierte Pakete können nicht gefunden werden.

Wenn bei der Installation Python und installierte Pakete nicht gefunden werden können, weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor, das während der Homebrew-Installation aufgetreten ist. Da die CLI nicht virtualenv verwendet, verlässt sie sich darauf, dass die richtigen, von Homebrew installierten Versionen von Python gefunden werden. Sie können diese Probleme vielleicht beheben, indem Sie die Python-Installation erneut verknüpfen:

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>Die CLI-Version ist veraltet.

Wenn die installierte CLI-Version Ihrer Meinung nach veraltet sein könnte, müssen Sie den Befehl `brew update` gefolgt von `brew upgrade azure-cli` ausführen. Wenn die CLI dadurch nicht aktualisiert wird, berücksichtigen Sie, dass das Rollout von Homebrew-Paketen unter Umständen langsamer erfolgen kann als das von allgemeinen Releases. Wenn Sie die aktuellste Version der CLI benötigen, sollten Sie sie [manuell installieren](#manage-the-cli-manually).

### <a name="uninstall-with-homebrew"></a>Deinstallieren mit Homebrew

Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten. Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können. Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist. Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).

Wenn Sie Homebrew für die Installation verwendet haben, sollten Sie Homebrew auch für die Deinstallation verwenden.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>Manuelles Installieren der CLI

Wenn Sie für die Verwaltung der CLI-Installation Homebrew nicht verwenden können oder möchten, können Sie eine manuelle Installation durchführen.

Befolgen Sie die [Anweisungen für die manuelle Linux-Installation](install-azure-cli-linux.md) für die manuelle Installation unter macOS. macOS-Version 10.9 und höhere Versionen müssen alle erforderlichen Abhängigkeiten enthalten.
