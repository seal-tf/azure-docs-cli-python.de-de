---
title: "Installieren der Azure-Befehlszeilenschnittstelle für Windows"
description: Installieren der Azure CLI 2.0 unter Windows
keywords: Azure CLI,Azure CLI installieren,Azure installieren Windows, Azure CLI Windows, Azure Windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fc84b80e44a994495ef97cf9d7ec4e4a79a5c5b3
ms.sourcegitcommit: b41c5ed4a26c771a1a32b4560131f7a65b80fd33
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/03/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Installieren der Azure CLI 2.0 unter Windows

Unter Windows wird die Binärdatei der Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.
Bei Verwendung des Windows-Subsystems für Linux (WSL) sind Pakete für Ihre Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen. In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Eingabeaufforderung nicht verfügbar sind.

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden. 

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
