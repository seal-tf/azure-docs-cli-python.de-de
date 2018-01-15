---
title: "Manuelle Installation der Azure CLI 2.0 für Linux"
description: Manuelle Installation der Azure CLI 2.0 unter Linux
keywords: Azure CLI,Azure CLI installieren,Azure Linux, Azure installieren Linux
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
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Manuelle Installation der Azure CLI 2.0 unter Linux

Wenn in Ihrer Distribution kein Paket für die Azure CLI enthalten ist, können Sie die CLI durch Ausführen eines Installationsskripts jederzeit manuell installieren. Sofern ein Paket verfügbar ist, ist dies jedoch stets die empfohlene Installationsmethode.

## <a name="prerequisites"></a>Voraussetzungen

Zum Installieren der CLI muss auf dem System folgende Software verfügbar sein:

* [Python 2.7 oder Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>Manuelles Installieren oder Aktualisieren

Sie müssen eine vollständige Installation ausführen – unabhängig davon, ob die CLI installiert oder aktualisiert wird. Wenn alle erforderlichen Komponenten vorhanden sind, können Sie die CLI durch Ausführung von `curl` installieren.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Wenn `curl` nicht auf Ihrem System vorhanden ist, können Sie auch das Skript herunterladen und lokal ausführen. Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden. Führen Sie nach der Installation die CLI mit dem Befehl `az` aus.

## <a name="troubleshooting"></a>Problembehandlung

### <a name="curl-object-moved-error"></a>curl-Fehler „Objekt verschoben“

Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Der Befehl `az` wurde nicht gefunden.

Wenn Sie nach der Installation den Befehl nicht ausführen können, müssen Sie unter Umständen den Befehlshash-Cache Ihrer Shell leeren. Ausführen

```bash
hash -r
```

und überprüfen, ob das Problem behoben ist.

Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben. Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.

Wenn Sie das Installationsskript ausgeführt haben:

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>Manuelles Deinstallieren

Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten. Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können. Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist. Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).

Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Installationsverzeichnis löschen. Das Installationsverzeichnis sollte zum Installationszeitpunkt ausgewählt worden sein, wenn die Installation über das Skript `https://aka.ms/InstallAzureCLI` erfolgt ist. Das Standardinstallationsverzeichnis ist `$HOME`.

Entfernen Sie zunächst die installierten CLI-Dateien:

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

Ändern Sie anschließend die Datei `$HOME/.bash_profile`, um folgende Zeile zu entfernen:

```
<install location>/lib/azure-cli/az.completion
```

Wenn Ihre Shell einen Befehlscache verwendet, laden Sie ihn erneut. `bash`- und `zsh`-Benutzer müssen den folgenden Schritt ausführen:

```bash
hash -r
```
