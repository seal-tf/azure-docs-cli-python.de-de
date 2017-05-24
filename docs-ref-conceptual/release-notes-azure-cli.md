---
title: Azure CLI 2.0-Versionshinweise
description: "Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0."
keywords: Azure CLI 2.0-Versionshinweise
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0-Versionshinweise

## <a name="may-10-2017"></a>10. Mai 2017

Version 2.0.6

* Umbenennen von „documentdb“ in „cosmosdb“
* Hinzufügen von rdbms (mysql, postgres)
* Einbeziehen der Data Lake Analytics- und Data Lake Store-Module
* Einbeziehen des Cognitive Services-Moduls
* Einbeziehen des Service Fabric-Moduls
* Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)
* Hinzufügen von Unterstützung für CDN-Befehle
* Entfernen des Containermoduls
* Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))
* Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))

```
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a>Core

* Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung   
* Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))
* Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))
* Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))
* Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))
* Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))
* Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))
* Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))
* Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))
* Core: Verbesserte Leistung
* Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen
* Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist

### <a name="acs"></a>ACS

* Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge
* Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung
* Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen
* Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.
* Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“
* Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)
* Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps
* Verfügbarmachen von „webapp list-runtimes“
* Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))
* Unterstützen des Slottauschs mit Vorschau
* Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))
* Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* Umbenennen des documentdb-Moduls in cosmosdb.
* Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung
* Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten
* Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst
* Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“ Zugriff über: `az dla catalog package`
* Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):

  * Table
  * Tabellenwertfunktion
  * Sicht
  * Tabellenstatistiken. Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.

### <a name="data-lake-store"></a>Data Lake Store

* Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird
* Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))
* Fehlende Hilfe für Zugriffsanzeige hinzugefügt ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Suchen

* Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen
* BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden
* Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben
* Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht
* Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Labor

* Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung
* Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor
* Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern
* Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors
* Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor

### <a name="monitor"></a>Überwachen

* Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Netzwerk

* Hinzufügen des `network watcher test-connectivity`-Befehls
* Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.
* Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich
* Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen
* Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln
* Hinzufügen von Unterstützung für geografisches TrafficManager-Routing
* Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen
* Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen
* Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.
* Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways
* Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen
* BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create` 
* Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde
* Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden
* Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte
* Hinzufügen von „network watcher“-Vorschaubefehlen

### <a name="profile"></a>Profil

* Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird
* Verwerfen des Befehls „update-settings“

### <a name="resource"></a>Ressource

* Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))
* Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))
* Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))
* Korrigieren der Ressourcenanalyse und der API-Versionssuche ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* Hinzufügen von Dokumenten für „az lock update“ ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Rolle

* create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))
* Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird

### <a name="sql"></a>SQL

* Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“
* SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Speicher

* Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`
* Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs
* Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs
* Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist

### <a name="vm"></a>VM

* avail-set: Festlegen der UD- und FD-Domänenanzahl als optional

  Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.
* vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren
* vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>3. April 2017

Version 2.0.2

In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.

```
azure-cli (2.0.2)
 
acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a>Core

* Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste
* Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))
* Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))
* Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))
* Hinzufügen der Meldung zu fehlenden Vorlagenparametern ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM
* Unterstützen der Anmeldung an einem bestimmten Mandanten
 
### <a name="acs"></a>ACS

* [ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))
* Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* Hinzufügen von Unterstützung für Windows-Cluster ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“ ([#2321](https://github.com/Azure/azure-cli/pull/2321))
 
### <a name="appservice"></a>AppService

* appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))
* appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))
* appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))
 
### <a name="datalake"></a>DataLake

* Erste Version des Data Lake Analytics-Moduls
* Erste Version des Data Lake Store-Moduls
 
### <a name="docuemntdb"></a>DocumentDB

* DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))
* Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27. Februar 2017

Version 2.0.0

Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.
Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:
- Container Service (acs)
- Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)
- Netzwerk
- Storage

Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.
Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.
Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden.
Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.

Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.

Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.
In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.

```
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)
 
Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32) 
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.
> Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.

Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.
Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).

Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:
- Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)
- Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`

