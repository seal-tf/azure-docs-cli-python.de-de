---
title: Azure CLI 2.0-Versionshinweise
description: "Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0."
keywords: Azure CLI 2.0-Versionshinweise
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 72630c52b5e6afd69809ff19145717c0d65e0252
ms.sourcegitcommit: 3a490ae3a2a1b2e63a062806f9b720fa4c6be01e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2017
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0-Versionshinweise

## <a name="september-22-2017"></a>22. September 2017

Version 2.0.18

### <a name="resource"></a>Ressource

* Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt
* Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt
* Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt
* [WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.

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

* Erste Version.

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

* Rechtlichen Hinweis zu `--version` hinzugefügt.

### <a name="acs"></a>ACS

* Vorschauregionen korrigiert.
* Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.
* ACS-Befehlsausgabe optimiert.

### <a name="appservice"></a>AppService

* [WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben
* Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt
* `az webapp log show` verfügbar gemacht
* Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten
* Behoben: Korrekte Erkennung der Sloteinstellungen

### <a name="iot"></a>IoT

* Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien

### <a name="network"></a>Netzwerk

* [WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt
* [WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt
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
* [WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt
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


### <a name="data-lake-store"></a>Data Lake-Speicher

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

### <a name="data-lake-store"></a>Data Lake-Speicher

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
* Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.
* Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt


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
Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.

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

