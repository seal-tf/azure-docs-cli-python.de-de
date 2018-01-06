---
title: "Installieren der Azure-Befehlszeilenschnittstelle für Windows"
description: Installieren der Azure CLI 2.0 unter Windows
keywords: Azure CLI,Azure CLI installieren,Azure installieren Windows, Azure CLI Windows, Azure Windows
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
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Installieren der Azure CLI 2.0 unter Windows

Unter Windows können Sie über ein MSI-Installationsprogramm eine native Binärdatei installieren, die über die Windows-Eingabeaufforderung oder PowerShell verwendet werden kann. Wenn Sie das Windows-Subsystem für Linux (WSL) ausführen, sind Pakete für die ausgeführte Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

## <a name="install-or-update-with-msi"></a>Installieren oder Aktualisieren mit MSI

Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet. Sie können das [MSI-Installationsprogramm herunterladen](https://aka.ms/InstallAzureCliWindows) und anschließend zum Installieren oder Aktualisieren ausführen.

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.

## <a name="uninstall-with-msi"></a>Deinstallieren mit der MSI-Datei

Es tut uns leid, wenn Sie die Azure CLI deinstallieren möchten. Teilen Sie uns vor der Deinstallation mithilfe des Befehls `az feedback` mit, warum Sie sich für die Deinstallation entschieden haben und wie wir die CLI verbessern können. Wir möchten sicherstellen, dass die Azure CLI möglichst fehlerfrei und benutzerfreundlich ist. Sie können auch ein [GitHub-Problem melden](https://github.com/Azure/azure-cli/issues).

Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden. Sie können das [MSI-Installationsprogramm herunterladen](https://aka.ms/InstallAzureCliWindows), wenn es nicht mehr auf Ihrem Computer verfügbar ist.
