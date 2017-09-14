---
title: Verwalten mehrerer Clouds mit der Azure CLI 2.0
description: "Die Azure CLI 2.0 ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei verschiedenen Clouds."
keywords: Azure CLI 2.0, Azure, Clouds, Datencenter, Regierung, Region, China, Deutschland
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Verwalten mehrerer Clouds mit der Azure CLI 2.0

Wenn mehrere Abonnements mit Azure verknüpft sind, stehen Ihnen unter Umständen mehrere Clouds zur Verfügung. Jede Cloud verfügt über eigene zugeordnete Endpunkte und Funktionen und ist häufig einer bestimmten Region zugeordnet, für die unterschiedliche Datenschutzstandards oder -anforderungen gelten.

Für die effektive Verwendung mehrerer Clouds müssen Sie die derzeit aktive Cloud wechseln und ggf. neue Clouds erstellen können.

## <a name="listing-clouds"></a>Auflisten von Clouds

Sie können die verfügbaren Clouds mit dem Befehl [cloud list](/cli/azure/cloud#list) auflisten. Dadurch erfahren Sie, welche Cloud derzeit aktiv ist und wie das aktuelle Profil lautet. Darüber hinaus werden Informationen zu regionalen Suffixen und Hostnamen bereitgestellt.

So rufen Sie eine Liste der verfügbaren Clouds und die derzeit aktive Cloud ab:

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

## <a name="switching-the-active-cloud"></a>Wechseln der aktiven Cloud

Um die derzeit aktive Cloud zu wechseln, führen Sie den Befehl [cloud set](/cli/azure/cloud#set) aus. Dieser Befehl erfordert ein Argument: den Namen der Cloud.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Wenn Sie sich nie für die aktive Cloud authentifiziert haben, müssen Sie dies vor dem Ausführen weiterer CLI-Vorgänge nachholen. Anleitungen zur Authentifizierung finden Sie unter [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli) (Anmelden bei der Azure CLI 2.0).

## <a name="register-or-unregister-a-cloud"></a>Registrieren oder Aufheben der Registrierung einer Cloud

Registrieren Sie eine neue Cloud, wenn Sie eigene Endpunkte besitzen oder ein anderes Profil benötigen. Eine Cloud wird mit dem Befehl [cloud register](/cli/azure/cloud#register) erstellt. Dieser Befehl erfordert einen Namen und optional einen Satz von Funktionen und Endpunktangaben.

So erstellen Sie eine Cloud mit einem spezialisierten Endpunkt für den Ressourcen-Manager und einem bestimmten Profil:

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

Dadurch wird die Cloud erstellt, aber _nicht_ automatisch ausgewählt.

Wenn Sie die erstellte Cloud nicht mehr benötigen, kann ihre Registrierung mit dem Befehl [cloud unregister](/cli/azure/cloud#unregister) aufgehoben werden:

```azurecli
az cloud unregister --name MyCloud
```

