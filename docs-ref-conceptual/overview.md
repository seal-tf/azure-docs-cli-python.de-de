---
title: Azure CLI 2.0
description: "Enthält eine Übersicht über Azure CLI 2.0."
keywords: Azure CLI 2.0, Linux, MacOS, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 35e754b4ecd75481bd60d95dd1545b798c2e85b3
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/16/2017
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 ist die neue Befehlszeilenumgebung von Azure und dient zum Verwalten von Azure-Ressourcen.  Sie kann unter MacOS, Linux und Windows verwendet werden. 

Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert. Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Lesen Sie im [Artikel zur Installation](install-azure-cli.md) nach, um die Azure CLI 2.0 auf Ihrem System einzurichten, oder verwenden Sie die [Cloud Shell](/azure/cloud-shell/overview) zum Ausführen der CLI in Ihrem Browser.
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