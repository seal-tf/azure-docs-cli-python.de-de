---
title: Azure CLI 2.0
description: "Enthält eine Übersicht über Azure CLI 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 5f3d514200b138d498043e0efb2cf5c2f478d108
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2018
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 ist die neue Befehlszeilenumgebung von Azure und dient zum Verwalten von Azure-Ressourcen.
Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux und Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.

Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert. Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Führen Sie die CLI mithilfe von [Cloud Shell](/azure/cloud-shell/overview) in Ihrem Browser aus, oder [installieren](install-azure-cli.md) Sie sie unter macOS, Linux oder Windows.
Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mit der Verwendung der CLI zu beginnen.
Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).

In den folgenden Beispielen werden gängige Szenarien mit Azure CLI 2.0 veranschaulicht:
- [Virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web-Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Außerdem ist eine ausführliche [Referenz](/cli/azure/) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.

Führen Sie jetzt die [ersten Schritte](get-started-with-azure-cli.md) mit Azure CLI 2.0 aus.


> [!NOTE]
> Falls Sie die vorherige Version der CLI (Azure-CLI) nutzen, können Sie sie weiterverwenden.
> Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).
