---
title: Azure CLI 2.0-Versionshinweise
description: Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 254c7b306440d921cef6b611268839150fdf3196
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0-Versionshinweise

## <a name="may-7-2018"></a>7. Mai 2018

Version 2.0.32

### <a name="core"></a>Core

* Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.
* Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt
* Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte [#5591](https://github.com/Azure/azure-cli/issues/5591)
* Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage
* Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten
* Fehler bei der Eingabe von `az ''` behandelt
* Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt

### <a name="acr"></a>ACR

* ACR Build-Befehle hinzugefügt
* Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert
* Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung
* ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert
* Fehlermeldungen zu Repositorybefehlen optimiert
* Tabellenspalten und -reihenfolge aktualisiert

### <a name="acs"></a>ACS

* Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist
* Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird

### <a name="ams"></a>AMS

* Erste Version: Verwalten von Azure Media Services-Ressourcen

### <a name="appservice"></a>AppService

* Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.
* `--runtime-version` aus `webapp auth update` entfernt
* Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt
* Unterstützung für mehrere Container hinzugefügt

### <a name="batch-ai"></a>Batch AI

* `batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.

### <a name="cognitive-services"></a>Cognitive Services

* Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))

### <a name="consumption"></a>Nutzung

* Neue Befehle für Budget-API hinzugefügt

### <a name="container"></a>Container

* `--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.

### <a name="cosmos-db"></a>Cosmos DB

* VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB

### <a name="dms"></a>DMS

* Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.

### <a name="extension"></a>Durchwahl

* Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden

### <a name="interactive"></a>Interactive

* Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.
* Benutzerfreundlichere Ausgabe bei der Eingabe von '\'
* Abschlüsse für Parameter ohne Hilfe korrigiert
* Beschreibungen für Befehlsgruppen korrigiert

### <a name="lab"></a>Labor

* Regressionen aus Knack-Umwandlung korrigiert

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE] Parameter `--ids` entfernt für: 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a>Profil

* Quellerkennung für `disk create` korrigiert
* [BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden
* Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert

### <a name="redis"></a>Redis

* `redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.
* `redis list-all` als veraltet markiert Diese Funktion wurde in `redis list` integriert.
* `redis import-method` wurde durch `redis import` ersetzt.
* Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt

### <a name="role"></a>Rolle

* [BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt

### <a name="storage"></a>Speicher

* Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden
* Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads
* Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln
* Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt
* `storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren

### <a name="vm"></a>VM

* Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert
* Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt
* [BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.
* Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt
* [BREAKING CHANGE] `--ids` entfernt aus:
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* Unterstützung für Schreibbeschleunigung hinzugefügt 
* `vmss perform-maintenance` hinzugefügt
* `vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen
* `vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen


## <a name="april-10-2018"></a>10. April 2018

Version 2.0.31

### <a name="acr"></a>ACR

* Verbesserte Fehlerbehandlung für wincred-Fallback

### <a name="acs"></a>ACS

* Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert

### <a name="appservice"></a>AppService

* [BREAKING CHANGE]: Removed `assign-identity`
* Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben

### <a name="batchai"></a>Batch AI

* Unterstützung für API 2018-03-01 hinzugefügt

 - Bereitstellung auf Auftragsebene
 - Umgebungsvariablen mit Geheimniswerten
 - Einstellungen von Leistungsindikatoren
 - Berichtstellung für auftragsspezifisches Pfadsegment
 - Unterstützung für Unterordner in Listendateien-API
 - Berichterstellung zur Nutzung und zu Grenzwerten
 - Zulassen der Angabe des Cachetyps für NFS-Server
 - Unterstützung für benutzerdefinierte Images
 - Unterstützung für pyTorch-Toolkit hinzugefügt

* Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet
* Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden
* Nationale Clouds werden unterstützt
* Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen
* Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images
* Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt
* Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht. Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).
* Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)
* Verbesserte `table`-Ausgabe für `show`-Vorgänge
* Option `--use-auto-storage` für die Clustererstellung hinzugefügt. Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.
* `--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt
* Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile
* [BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben
* [BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen

### <a name="billing"></a>Abrechnung

* Registrierungskontobefehle hinzugefügt

### <a name="consumption"></a>Nutzung

* Befehle vom Typ `marketplace` hinzugefügt
* [BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt
* [BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt
* [BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt
* [BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt
* [BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt

### <a name="container"></a>Container

* Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt
* [#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde

### <a name="extension"></a>Durchwahl

* Meldung für Distributionsüberprüfung in Debugebene geändert

### <a name="interactive"></a>Interactive

* Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen
* Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt
* Abschluss für `--ids`-Parameter hinzugefügt

### <a name="network"></a>Netzwerk

* [#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden
* Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt. [#4910](https://github.com/Azure/azure-cli/issues/4910)
* `ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt 
* Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen
* Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben
* Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt
* Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt

### <a name="profile"></a>Profil

* Unterstützung für klassische Azure-Konten in `account list` hinzugefügt
* [BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt

### <a name="rdbms"></a>RDBMS

* Befehl `georestore` hinzugefügt
* Speichergrößenbeschränkung aus Befehl `create` entfernt

### <a name="resource"></a>Ressource

* Unterstützung für `--metadata` zu `policy definition create` hinzugefügt
* Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt

### <a name="sql"></a>SQL

* `sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt

### <a name="storage"></a>Speicher

* Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert

### <a name="vm"></a>VM

* Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt
* `vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt
* Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann. [#5718](https://github.com/Azure/azure-cli/issues/5718)
* Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist


## <a name="march-27-2018"></a>27. März 2018

Version 2.0.30

### <a name="core"></a>Core

* Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind

### <a name="acs"></a>ACS

* Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell

### <a name="appservice"></a>AppService

* Unterstützung nur von HTTPS zu `webapp update` hinzugefügt
* Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt

### <a name="backup"></a>Backup

* Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt. Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.
* Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* `--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.

### <a name="container"></a>Container

* Befehl `container exec` hinzugefügt. Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe
* Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe

### <a name="extension"></a>Durchwahl

* Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet
* `extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen
* [BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen

### <a name="interactive"></a>Interactive

* Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.
* Fehler bei der Verwendung des Parameters `--style` behoben
* Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)
* Verbesserte Unterstützung der Vervollständigung

### <a name="lab"></a>Labor

* Probleme mit Befehl `create environment` behoben

### <a name="monitor"></a>Überwachen

* Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))
* [#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.
* Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))

### <a name="network"></a>Netzwerk

* Unterstützung für private DNS-Zonen hinzugefügt

### <a name="profile"></a>Profil

* Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt

### <a name="rdbms"></a>RDBMS

* GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt

### <a name="resource"></a>Ressource

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Rolle

* Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt
* `rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben
* Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt
* [BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt
* Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt

### <a name="storage"></a>Speicher

* Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben
* [#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten

### <a name="vm"></a>VM

* Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt
* Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt
* Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden
* [BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben

## <a name="march-13-2018"></a>13. März 2018

Version 2.0.29

### <a name="acr"></a>ACR

* Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt
* Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert
* Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt

### <a name="acs"></a>ACS

* Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt
* `kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert

### <a name="advisor"></a>Advisor

* [BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt
* [BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt
* [BREAKING CHANGE] `advisor recommendation generate` entfernt 
* Parameter `--refresh` zu `advisor recommendation list` hinzugefügt
* Befehl `advisor recommendation show` hinzugefügt

### <a name="appservice"></a>AppService

* `[webapp|functionapp] assign-identity` als veraltet markiert
* Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt

### <a name="eventhubs"></a>Event Hubs

* Erste Version

### <a name="extension"></a>Durchwahl

* Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann

### <a name="interactive"></a>Interactive

* [#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten
* [#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt
* [#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat
* Statusanzeige für lang ausgeführte Vorgänge korrigiert

### <a name="monitor"></a>Überwachen

* `monitor autoscale-settings`-Befehle als veraltet markiert
* Befehle vom Typ `monitor autoscale` hinzugefügt
* Befehle vom Typ `monitor autoscale profile` hinzugefügt
* Befehle vom Typ `monitor autoscale rule` hinzugefügt

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt
* Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* `network watcher connection-monitor`-Befehle hinzugefügt
* Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt

### <a name="profile"></a>Profil

* Parameter `--msi` für `az login` als veraltet markiert
* Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt

### <a name="rdbms"></a>RDBMS

* [VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird

### <a name="service-bus"></a>Service Bus

* Erste Version

### <a name="storage"></a>Speicher

* [#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.
* [#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.

### <a name="vm"></a>VM

* `[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.
* `[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert
* Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt
* Standardpriorität in `vmss create` auf „Keine“ geändert

## <a name="february-27-2018"></a>27. Februar 2018

Version 2.0.28

### <a name="core"></a>Core

* [5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben
* Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt
* HTTP-Protokollierung zu `--debug` hinzugefügt

### <a name="acs"></a>ACS

* Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird
* Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe
* Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt
* Veraltungshinweis aus `aks get-versions` entfernt

### <a name="appservice"></a>AppService

* Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)
* [5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.

### <a name="cognitive-services"></a>Cognitive Services

* Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert

### <a name="consumption"></a>Nutzung

* Neue Befehle für PriceSheet-API hinzugefügt
* Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert

### <a name="container"></a>Container

* Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können

### <a name="network"></a>Netzwerk

* [5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Ressource

* `group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war

### <a name="role"></a>Rolle

* `role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen

### <a name="sql"></a>SQL

* Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)

### <a name="storage"></a>Speicher

* Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht

### <a name="vm"></a>VM

* Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt


## <a name="february-13-2018"></a>13. Februar 2018

Version 2.0.27

### <a name="core"></a>Core

* Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert

### <a name="acs"></a>ACS

* [BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt
* `aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert
* Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert
* Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert
* Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert
* Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert
* `aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln
* Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern

### <a name="appservice"></a>AppService

* Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte
* Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt

### <a name="cdn"></a>CDN

* Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt

### <a name="container"></a>Container

* Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt
* Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt

### <a name="cosmosdb"></a>CosmosDB

* Unterstützung für Einstellungsfunktionen hinzugefügt

### <a name="extension"></a>Durchwahl

* Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt
* Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt

### <a name="feedback"></a>Feedback

* Erweiterungsinformationen zu Telemetriedaten hinzugefügt

### <a name="interactive"></a>Interactive

* Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird
* Regression mit fehlenden Parametervervollständigungen korrigiert

### <a name="iot"></a>IoT

* Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt
* Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt
* Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt
* `iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen

### <a name="monitor"></a>Überwachen

* Befehl `az monitor log-profiles create` korrigiert

### <a name="network"></a>Netzwerk

* Option `--tags` für folgende Befehle korrigiert:
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a>Profil

* `az login` im interaktiven Modus aktiviert

### <a name="resource"></a>Ressource

* `feature show` wieder hinzugefügt

### <a name="role"></a>Rolle

* Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt

### <a name="sql"></a>SQL

* Befehle vom Typ `sql server dns-alias` hinzugefügt
* `sql db rename` hinzugefügt
* Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt

### <a name="storage"></a>Speicher

* Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen

### <a name="vm"></a>VM

* Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben
* Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt
* `vm boot-diagnostics get-boot-log` (feststehend)


## <a name="january-31-2018"></a>31. Januar 2018

Version 2.0.26

### <a name="core"></a>Core

* Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt
* Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt
* Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde. `--verbose` zum Anzeigen verwenden.
* Statusanzeige für Wait-Befehle hinzugefügt

### <a name="acs"></a>ACS

* Argument `--disable-browser` erläutert
* Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert

### <a name="appservice"></a>AppService

* `webapp log [tail|download]` (feststehend)
* Überprüfung `kind` für Web-Apps und Funktionen entfernt

### <a name="cdn"></a>CDN

* Problem mit fehlendem Client für `cdn custom-domain create` behoben

### <a name="cosmosdb"></a>CosmosDB

* Parameterbeschreibung für Failoverrichtlinien korrigiert

### <a name="interactive"></a>Interactive

* Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden

### <a name="network"></a>Netzwerk

* Schutz für `--cert-password` zu `application-gateway create` hinzugefügt
* Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete
* Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt
* Problem mit fehlendem Client für `asg create` behoben
* Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt
* Folgende Probleme mit `dns zone export` behoben:
  * Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden
  * Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden
* Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden 
* Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt

### <a name="profile"></a>Profil

* `get-access-token` zur Verwendung auf einer VM mit Identität korrigiert

### <a name="resource"></a>Ressource

* Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt

### <a name="storage"></a>Speicher

* Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben
* Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt
* Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat  
* Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt
* Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten

### <a name="vm"></a>VM

* Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen
* `[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können
* [VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt
* Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt


## <a name="january-17-2018"></a>17. Januar 2018

Version 2.0.25

### <a name="acr"></a>ACR

* Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt
* Registrierungsprotokolle aktiviert

### <a name="acs"></a>ACS

* Befehl `get-credentials` korrigiert
* SPN-Rollenanforderung entfernt

### <a name="appservice"></a>AppService

* Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war
* Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt
* Slotunterstützung für `log tail` korrigiert

### <a name="backup"></a>Backup

* Option `--container-name` von `backup item list` geändert (ist jetzt optional)
* Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt
* Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)
* Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat
* `backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)

### <a name="batch"></a>Batch

* `batch login` geändert, um Authentifizierungsdetails zurückzugeben

### <a name="cloud"></a>Cloud

* Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.

### <a name="consumption"></a>Nutzung

* Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`

### <a name="event-grid"></a>Event Grid

* [BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.
* [BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.
* [BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt. Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.
* Befehl `eventgrid topic update` hinzugefügt
* Befehl `eventgrid event-subscription update` hinzugefügt
* Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt
* Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt

### <a name="interactive"></a>Interactive

* Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte
* Fehler beim Start behoben
* Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten

### <a name="iot"></a>IoT

* Unterstützung für Gerätebereitstellungsdienst hinzugefügt
* Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt
* IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren

### <a name="monitor"></a>Überwachen

* Unterstützung mehrerer Diagnoseeinstellung hinzugefügt. Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.
* Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt

### <a name="network"></a>Netzwerk

* Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat
* Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt

### <a name="profile"></a>Profil

* Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt

### <a name="role"></a>Rolle

* Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen

### <a name="service-fabric"></a>Service Fabric

* Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt
* Problem mit fehlendem Client für verschiedene Befehle behoben

### <a name="vm"></a>VM

* [VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`
* [BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert
* [BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI
* [VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt
* Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt
* Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt
* Fehlerbedingte Probleme mit `[vm|vmss] create` behoben
* Übermäßige Ressourcenverwendung durch `vm image list --all` behoben

## <a name="december-19-2017"></a>19. Dezember 2017

Version 2.0.23

* Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt

### <a name="container"></a>Container

* Falsche Reihenfolge der Parameter für Containerprotokolle behoben

### <a name="network"></a>Netzwerk

* Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt
* Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt

### <a name="storage"></a>Speicher

* Unterstützung für Storage V2 hinzugefügt

### <a name="vm"></a>VM

* [VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt


## <a name="december-5-2017"></a>5. Dezember 2017

Version 2.0.22

* `az component`-Befehle wurden entfernt. Verwenden Sie stattdessen `az extension`.

### <a name="core"></a>Core
* Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.
* Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden

### <a name="acs"></a>ACS

* Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.
* Verbesserte Fehlerberichterstellung für `acs create`
* Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad

### <a name="advisor"></a>Advisor

* Erste Version

### <a name="appservice"></a>AppService

* Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`
* `webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen
* Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt

### <a name="consumption"></a>Nutzung

* Unterstützung für API-Version 2017-11-30 hinzugefügt

### <a name="container"></a>Container

* Feste Regression für Standardports

### <a name="monitor"></a>Überwachen

* Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt

### <a name="resource"></a>Ressource

* Argument `--include-response-body` zu `resource show` hinzugefügt

### <a name="role"></a>Rolle

* Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt
* Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt
* Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`

### <a name="sql"></a>SQL

* Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.
* Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.

### <a name="vm"></a>VM

* Zoneninformationen zu `az vm list-skus` hinzugefügt


## <a name="november-14-2017"></a>14. November 2017

Version 2.0.21

### <a name="acr"></a>ACR

* Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt


### <a name="acs"></a>ACS

* Formulierung in AKS von „Agent“ in „Knoten“ geändert
* Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet
* VM-Standardgröße für AKS in `Standard_D1_v2` geändert
* `az aks browse` für Windows korrigiert
* `az aks get-credentials` für Windows korrigiert

### <a name="appservice"></a>AppService

* Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt
* Option `--docker-container-logging` zu `az webapp log config` hinzugefügt
* Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt
* Fehlermeldungen für `deployment user set` verbessert
* Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt
* `list-locations` (feststehend)

### <a name="batch"></a>Batch

* Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist

### <a name="batchai"></a>BatchAI

* Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt
* Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt
* Dokumentation für `job list-files` und `job stream-file` korrigiert
* Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt

### <a name="cloud"></a>Cloud

* `cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern

### <a name="container"></a>Container

* Unterstützung für das Öffnen mehrerer Ports hinzugefügt
* Neustartrichtlinie für Containergruppen hinzugefügt
* Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt
* Hilfedokumente aktualisiert

### <a name="data-lake-analytics"></a>Data Lake Analytics

* `[job|account] list` geändert, um präzisere Informationen zu erhalten

### <a name="data-lake-store"></a>Data Lake Store

* `account list` geändert, um präzisere Informationen zu erhalten

### <a name="extension"></a>Durchwahl

* `extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen
* `--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen

### <a name="iot"></a>IoT

* Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt

### <a name="monitor"></a>Überwachen

* Befehle vom Typ `activity-log alert` hinzugefügt

### <a name="network"></a>Netzwerk

* Unterstützung für CAA-DNS-Einträge hinzugefügt
* Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten
* Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte
* Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden

### <a name="reservations"></a>Reservations

* Erste Vorschauversion

### <a name="resource"></a>Ressource

* Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt

### <a name="sql"></a>SQL

* Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt

### <a name="storage"></a>Speicher

* `storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird
* Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten
* Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat
* Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt
* Problem beim Aktivieren von Metriken mit `storage metrics update` behoben
* Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben
* Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden

### <a name="vm"></a>VM

* Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat
* `--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt
* Befehle hinzugefügt: `vm secret `[add|remove|list]
* `vm format-secret` in `vm secret format` umbenannt
* Argument `--encrypt format` zu `vm encryption enable` hinzugefügt

## <a name="october-24-2017"></a>24. Oktober 2017

Version 2.0.20

### <a name="core"></a>Core

* Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API

### <a name="acr"></a>ACR

* Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.
* SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.
* Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.

### <a name="acs"></a>ACS

* [VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt
* Problem mit `get-credentials` in Kubernetes behoben

### <a name="appservice"></a>AppService

* Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren

### <a name="component"></a>Komponente

* Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt

### <a name="monitor"></a>Überwachen

* Befehle vom Typ `action-group` hinzugefügt

### <a name="resource"></a>Ressource

* Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben
* Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann

### <a name="vm"></a>VM

* Argument `--accelerated-networking` zu `vmss create` hinzugefügt


## <a name="october-9-2017"></a>9. Oktober 2017

Version 2.0.19

### <a name="core"></a>Core

* Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.

### <a name="appservice"></a>AppService

* Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.

### <a name="batch"></a>Batch

* Aktualisierung auf Batch SDK 4.0.0
* Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.
* Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt
* Batch-Unterstützung aus dem Komponentenmodell entfernt

### <a name="batchai"></a>BatchAI

* Erste Version des Batch AI-Moduls

### <a name="keyvault"></a>KeyVault

* Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>Netzwerk

* Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.
* `traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.

### <a name="resource"></a>Ressource

* Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt
* Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.
* Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.
* Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.

### <a name="sql"></a>Sql

* Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt
* Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.
* `db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.

### <a name="storage"></a>Speicher

* Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt

### <a name="vm"></a>VM

* Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte
* [VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt
* Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt
* Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt
* Parameter `--license-type` für Windows zu `vmss create` hinzugefügt


## <a name="september-22-2017"></a>22. September 2017

Version 2.0.18

### <a name="resource"></a>Ressource

* Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt
* Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt
* Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt
* [BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.

### <a name="network"></a>Netzwerk

* Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt
* Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt
* Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt
* Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt
* Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt
* Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt
* Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt

### <a name="storage"></a>Speicher

* Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte

### <a name="eventgrid"></a>Eventgrid

* Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert

### <a name="sql"></a>SQL

* `sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist. Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.
* Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt

### <a name="keyvault"></a>KeyVault

* Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt

### <a name="vm"></a>VM

* Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt
* Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte
* Argument `--asgs` zu `vm create` hinzugefügt
* Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt
* [VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt
* Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt

### <a name="acs"></a>ACS

* [VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt

### <a name="appservice"></a>AppService

* Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`

### <a name="backup"></a>Backup

* Vorschauversion


## <a name="september-11-2017"></a>11. September 2017

Version 2.0.17

### <a name="core"></a>Core

* Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert
* Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat

### <a name="acs"></a>ACS

* Befehl `acs list-locations` hinzugefügt
* `ssh-key-file` wird mit dem erwarteten Standardwert versehen.

### <a name="appservice"></a>AppService

* Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs

### <a name="cdn"></a>CDN

* Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.

### <a name="extension"></a>Durchwahl

* Erste Version

### <a name="keyvault"></a>KeyVault

* Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste

### <a name="network"></a>Netzwerk

* `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt
* Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.
* Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt
* Unterstützung für SKU zu `lb create` hinzugefügt
* Unterstützung für SKU zu `public-ip create` hinzugefügt

### <a name="resource"></a>Ressource

* Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen
* Übergabe von Parameterwerten für `policy assignment create` zulassen
* Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen
* Inkrementierte API-Version

### <a name="sql"></a>SQL

* Befehle vom Typ `sql server vnet-rule` hinzugefügt

### <a name="vm"></a>VM

* Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird
* Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden
* `subscription` aus der Ausgabe von `[vm|vmss] create` entfernt
* Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.
* Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.

## <a name="august-31-2017"></a>31. August 2017

Version 2.0.16

### <a name="keyvault"></a>KeyVault

* Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen

### <a name="sf"></a>Sf

* Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.

### <a name="storage"></a>Speicher

* Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen
* Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind

## <a name="august-28-2017"></a>28. August 2017

Version 2.0.15

### <a name="cli"></a>Befehlszeilenschnittstelle (CLI)

* Rechtlichen Hinweis zu `--version` hinzugefügt

### <a name="acs"></a>ACS

* Vorschauregionen korrigiert
* Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert
* ACS-Befehlsausgabe optimiert

### <a name="appservice"></a>AppService

* [BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben
* Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt
* `az webapp log show` verfügbar gemacht
* Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten
* Behoben: Korrekte Erkennung der Sloteinstellungen

### <a name="iot"></a>IoT

* Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt
* [BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt
* Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt
* Unterstützung für SKU zu `lb create` hinzugefügt
* Unterstützung für SKU zu `public-ip create` hinzugefügt

### <a name="profile"></a>Profil

* `--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht

### <a name="service-fabric"></a>Service Fabric

* Vorschauversion
* Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht
* Kennwortanforderung für Benutzer trotz Parameterübergabe behoben
* Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt

### <a name="storage"></a>Speicher

* Festlegen des Blobtarifs ermöglicht
* Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt
* Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt
* Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht
* [BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt
* Behoben (4220): `az storage account update encryption` – Syntaxkonflikt

### <a name="vm"></a>VM

* Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden
* Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:
* Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt
* Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten
* Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben
* Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte


## <a name="august-15-2017"></a>15. August 2017

Version 2.0.14

### <a name="acs"></a>ACS

* sshMaster0-Portnummer für Kubernetes korrigiert

### <a name="appservice"></a>AppService

* Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben

### <a name="event-grid"></a>Event Grid

* SDK-Abhängigkeiten hinzugefügt

## <a name="august-11-2017"></a>11. August 2017

Version 2.0.13

### <a name="acs"></a>ACS

* Weitere Vorschauregionen hinzugefügt

### <a name="batch"></a>Batch

* Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert
* Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt
* Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben
* Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“
* Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag
* Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt

### <a name="component"></a>Komponente

* Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt

### <a name="container"></a>Container

* `create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war


### <a name="data-lake-store"></a>Data Lake Store

* Fortschrittsüberwachung ermöglicht

### <a name="event-grid"></a>Event Grid

* Erste Version

### <a name="network"></a>Netzwerk

* `lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden
* `application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde
* `application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte
* Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`

### <a name="profile"></a>Profil

* `account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren

### <a name="storage"></a>Speicher

* Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht

### <a name="vm"></a>VM

* `availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht
* Befehl `list-skus` verfügbar gemacht
* Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen
* Anwenden von Speicher-SKU beim Anfügen von Datenträgern
* Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt


## <a name="july-28-2017"></a>28. Juli 2017

Version 2.0.12

* Containerbefehle hinzugefügt
* Abrechnungs- und Nutzungsmodule hinzugefügt

```
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a>Core

* Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten
* Ausnahmen beim Bereitstellungsfortschritt behoben
* Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients
* Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)
* Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung
* Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)
* Statusmeldung für Vorlagenbereitstellungen (3510)
* Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)
* Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)
* Erstellung von Abonnementclients mit richtigem SDK-Profil
* Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner
* Idempotenz für VM-/VMSS-Erstellung behoben (3586)
* Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.
* Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.
* Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack
* Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)

### <a name="acr"></a>ACR

* Befehl `show-usage` für verwaltete Registrierungen hinzugefügt
* Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen
* Verwaltete Registrierungen mit verwalteter SKU hinzugefügt
* Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt
* AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt
* Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt

### <a name="acs"></a>ACS

* Unterstützung der API-Version 2017-07-01

### <a name="appservice"></a>AppService

* Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat
* Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR
* Entfernung aller Befehle unter `appservice web`
* Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)
* Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)
* Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)
* Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)
* Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)
* Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt. Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.

### <a name="batch"></a>Batch

* Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert
* `pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt
* `pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt

### <a name="cdn"></a>CDN

* Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist

### <a name="cloud"></a>Cloud

* API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt
* Katalogendpunkt nicht erforderlich
* Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt
* Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können
* `endpoint_vm_image_alias_doc` verfügbar gemacht

### <a name="cosmosdb"></a>CosmosDB

* Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben
* Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt
* `dla job pipeline show` hinzugefügt
* `dla job recurrence list` hinzugefügt

### <a name="data-lake-store"></a>Data Lake Store

* Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt
* Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln
* Befehl `dls enable-key-vault` hinzugefügt. Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.

### <a name="interactive"></a>Interaktiv

* Startzeit durch Verwendung zwischengespeicherter Befehle verbessert
* Testabdeckung verbessert
* ?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird
* Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)
* `--version` als Parameter für den interaktiven Modus zugelassen (3645)
* Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)
* Statusmeldung für Vorlagenbereitstellungen (3510)
* Flag `--progress` hinzugefügt
* `--debug` und `--verbose` aus Abschlüssen entfernt
* `interactive` aus Abschlüssen entfernt (3324)

### <a name="iot"></a>IoT

* Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien (3934)

### <a name="key-vault"></a>Schlüsseltresor

* Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:
  * `keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`
  * `keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`
  * `keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`
  * `keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`
* Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)
* Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert (3307)

### <a name="lab"></a>Labor

* Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt
* Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt

### <a name="monitor"></a>Überwachen

* Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)
* `monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt
* `monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt
* `monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt
* `monitor alert-rules` in `monitor alert` umbenannt
* `monitor alert create` geändert:
  * Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.
  * Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung
  * `location` nicht mehr erforderlich
  * Hinzufügung von Namen- und ID-Unterstützung für Ziel
  * Entfernung von `--alert-rule-resource-name`
  * Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)
  * `description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.
  *  Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats
* Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`
* Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt

### <a name="network"></a>Netzwerk

* Befehl `list-private-access-services` hinzugefügt
* Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt
* Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte
* Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte
* Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist
* Befehle vom Typ `application-gateway redirect-config` hinzugefügt
* Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`
* Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`
* Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`
* Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt
* Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt
* Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt
* Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt
* Argument `--internal-dns-name-suffix` von `nic create` entfernt
* Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt
* Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde
* Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt
* Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert
* Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten
* Fehler mit Standardlogik von `network watcher show-topology` korrigiert
* Ausgabeformatierung für `network list-usages` verbessert
* Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)
* Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)
* Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)
* Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)

### <a name="profile"></a>Profil

* Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität
* Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat
* Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“
* Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt
* Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements

### <a name="rdbms"></a>RDBMS

* Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)
* Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)
* Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)
* MySQL- und PostgreSQL-Hilfe korrigiert (3369)

### <a name="resource"></a>Ressource

* Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert
* Analyse der Syntax `--parameters KEY=VALUE` verbessert
* Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden
* Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`
* Einige Analyse- und Fehlermeldungen korrigiert (3584)
* Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden
* Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)
* Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt

### <a name="role"></a>Rolle

* Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`
* Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)
* Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente
* Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`
* Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt

### <a name="service-fabric"></a>Service Fabric
* Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)
* Tests für Service Fabric-Befehle hinzugefügt (3424)
* Zahlreiche Service Fabric-Befehle korrigiert (3234)

### <a name="sql"></a>SQL

* Fehlerhaften Parameter `--identity` für `sql server create` entfernt
* Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt
* Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt

### <a name="storage"></a>Speicher

* Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)
* Erstellung eines reinen HTTPS-Speicherkontos ermöglicht
* Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)
* Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)
* Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)
* Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)

### <a name="vm"></a>VM

* Unterstützung der NSG-Konfiguration
* Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde
* Unterstützung verwalteter Dienstidentitäten
* Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte
* Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt


## <a name="may-10-2017"></a>10. Mai 2017

Version 2.0.6

* Umbenennen von „documentdb“ in „cosmosdb“
* Hinzufügen von rdbms (mysql, postgres)
* Einbeziehen der Data Lake Analytics- und Data Lake Store-Module
* Einbeziehen des Cognitive Services-Moduls
* Einbeziehen des Service Fabric-Moduls
* Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)
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

* Umbenennen des documentdb-Moduls in cosmosdb
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
* Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`
* Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich
* Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen
* Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln
* Hinzufügen von Unterstützung für geografisches TrafficManager-Routing
* Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen
* Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen
* Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`
* Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways
* Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen
* BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`
* Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde
* Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden
* Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte
* Hinzufügen von Network Watcher-Vorschaubefehlen

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
* Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))
* Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27. Februar 2017

Version 2.0.0

Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:
- Container Service (acs)
- Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)
- Netzwerk
- Speicher

Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.

Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.

Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.

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
> Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.

Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).

Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:
- Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)
- Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`

