---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI 2.0 unter Windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 30b9621c82af259e3de762127fd20b31eb249234
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Installieren der Azure CLI 2.0 unter Windows

Unter Windows wird die Binärdatei der Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.
Bei Verwendung des Windows-Subsystems für Linux (WSL) sind Pakete für Ihre Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://aka.ms/installazurecliwindows)

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen. In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind. Führen Sie den Befehl `az login` aus, um sich anzumelden.

```azurecli
az login
```

Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://aka.ms/installazurecliwindows)
