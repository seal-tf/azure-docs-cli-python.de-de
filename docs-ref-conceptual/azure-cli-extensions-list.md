---
title: Verfügbare Erweiterungen für die Azure CLI 2.0
description: Eine vollständige Liste der offiziell unterstützten Erweiterungen für die Azure CLI 2.0
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/26/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 04dbb4984c1fb2e43fe0aada76f851f3fd7b05b5
ms.sourcegitcommit: d461e73abb09c3c85064c532b53a2efb25833b01
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Verfügbare Erweiterungen für die Azure CLI 2.0

Dieser Artikel enthält eine vollständige Liste der verfügbaren Erweiterungen für die Azure CLI 2.0, die von Microsoft angeboten und unterstützt werden.

Die Liste der Erweiterungen ist auch direkt über die CLI verfügbar. Führen Sie zum Abrufen [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) aus:

```azurecli
az extension list-available --output table
```

| NAME | Version | Zusammenfassung | Vorschau |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Verwalten der Azure-Erweiterungen zur verbesserten Überwachung für SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Unterstützung für Befehlsaliase | Ja |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.2.1 | Zusätzliche Befehle für die Verwendung des Azure Batch-Diensts |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.3 | Stellt die Befehlsebene der Datenebene für Azure IoT Hub, IoT Edge und den IoT Device Provisioning-Dienst bereit |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Eine Azure CLI-Erweiterung für DNS-Zonen |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Eine Azure CLI-Erweiterung zum Kopieren von Images zwischen Regionen |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.1 | Zeigen Sie eine Vorschau der Azure Key Vault-Befehle an. | Ja |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Eine Azure CLI-Erweiterung für Verwaltungsgruppen |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Unterstützung für Verwaltungspartner (Vorschauversion) |  |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Eine Azure CLI-Erweiterung zur Bereitstellung der Unterstützung für Azure MySQL und Azure PostgreSQL |  |
| [SignalR](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Unterstützung für die SignalR-Verwaltung (Vorschauversion) | Ja |
| [Abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Unterstützung für die Abonnementverwaltung (Vorschauversion) |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Eine Azure CLI-Erweiterung zum Verwalten von appservice-Ressourcen | Ja |
