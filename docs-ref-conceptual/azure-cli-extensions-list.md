---
title: Verfügbare Erweiterungen für die Azure CLI 2.0
description: Eine vollständige Liste der offiziell unterstützten Erweiterungen für die Azure CLI 2.0
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ceca7ed92435ab03b196e60dee37195330f6f3c7
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Verfügbare Erweiterungen für die Azure CLI 2.0

Dieser Artikel enthält eine vollständige Liste der verfügbaren Erweiterungen für die Azure CLI 2.0, die von Microsoft angeboten und unterstützt werden.

Die Liste der Erweiterungen ist auch direkt über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli
az extension list-available --output table
```

| NAME | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Unterstützung für Befehlsaliase |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.1.0 | Zusätzliche Vorschauversionen von Azure Batch-Befehlen |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.1 | Stellt die Befehlsebene der Datenebene für Azure IoT Hub, IoT Edge und IoT Device Provisioning-Dienst bereit. |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Unterstützung für die öffentliche Vorschau des privaten Azure-DNS |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Kopieren von Images zwischen Regionen |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die Vorschauversion von Verwaltungsgruppen | Ja |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die Vorschauversion von Verwaltungspartnern | Ja |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.4 | Unterstützung für Azure MySQL und Azure PostgreSQL |  |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die Vorschauversion der Abonnementdefinitionen | Ja |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Erstellen und Bereitstellen von AppService-Ressourcen | Ja |
