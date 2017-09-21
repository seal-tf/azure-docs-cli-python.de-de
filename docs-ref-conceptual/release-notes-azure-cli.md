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
ms.openlocfilehash: 39e4710a29ac57730919b82ab76b9c9a4b9ca786
ms.sourcegitcommit: 43d4f838d132ab9bcfa59dbda3b544c06373b6a9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="bff08-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="bff08-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-15-2017"></a><span data-ttu-id="bff08-105">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-105">August 15, 2017</span></span>

<span data-ttu-id="bff08-106">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="bff08-106">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="bff08-107">ACS</span><span class="sxs-lookup"><span data-stu-id="bff08-107">ACS</span></span>

* <span data-ttu-id="bff08-108">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="bff08-108">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="bff08-109">AppService</span><span class="sxs-lookup"><span data-stu-id="bff08-109">Appservice</span></span>

* <span data-ttu-id="bff08-110">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="bff08-110">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="bff08-111">Event Grid</span><span class="sxs-lookup"><span data-stu-id="bff08-111">Event Grid</span></span>

* <span data-ttu-id="bff08-112">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-112">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="bff08-113">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-113">August 11, 2017</span></span>

<span data-ttu-id="bff08-114">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="bff08-114">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="bff08-115">ACS</span><span class="sxs-lookup"><span data-stu-id="bff08-115">ACS</span></span>

* <span data-ttu-id="bff08-116">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-116">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="bff08-117">Batch</span><span class="sxs-lookup"><span data-stu-id="bff08-117">Batch</span></span>

* <span data-ttu-id="bff08-118">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="bff08-118">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="bff08-119">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-119">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="bff08-120">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="bff08-120">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="bff08-121">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="bff08-121">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="bff08-122">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="bff08-122">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="bff08-123">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-123">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="bff08-124">Komponente</span><span class="sxs-lookup"><span data-stu-id="bff08-124">Component</span></span>

* <span data-ttu-id="bff08-125">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-125">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="bff08-126">Container</span><span class="sxs-lookup"><span data-stu-id="bff08-126">Container</span></span>

* <span data-ttu-id="bff08-127">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="bff08-127">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="bff08-128">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="bff08-128">Data Lake Store</span></span>

* <span data-ttu-id="bff08-129">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="bff08-129">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="bff08-130">Event Grid</span><span class="sxs-lookup"><span data-stu-id="bff08-130">Event Grid</span></span>

* <span data-ttu-id="bff08-131">Erste Version</span><span class="sxs-lookup"><span data-stu-id="bff08-131">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="bff08-132">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="bff08-132">Network</span></span>

* <span data-ttu-id="bff08-133">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="bff08-133">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="bff08-134">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="bff08-134">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="bff08-135">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="bff08-135">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="bff08-136">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="bff08-136">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="bff08-137">Profil</span><span class="sxs-lookup"><span data-stu-id="bff08-137">Profile</span></span>

* <span data-ttu-id="bff08-138">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="bff08-138">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="bff08-139">Speicher</span><span class="sxs-lookup"><span data-stu-id="bff08-139">Storage</span></span>

* <span data-ttu-id="bff08-140">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="bff08-140">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="bff08-141">VM</span><span class="sxs-lookup"><span data-stu-id="bff08-141">VM</span></span>

* <span data-ttu-id="bff08-142">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="bff08-142">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="bff08-143">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="bff08-143">Exposed `list-skus` command</span></span>
* <span data-ttu-id="bff08-144">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="bff08-144">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="bff08-145">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="bff08-145">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="bff08-146">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="bff08-146">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="bff08-147">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-147">July 28, 2017</span></span>

<span data-ttu-id="bff08-148">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="bff08-148">Version 2.0.12</span></span>

* <span data-ttu-id="bff08-149">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-149">Added container commands</span></span>
* <span data-ttu-id="bff08-150">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-150">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="bff08-151">Core</span><span class="sxs-lookup"><span data-stu-id="bff08-151">Core</span></span>

* <span data-ttu-id="bff08-152">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="bff08-152">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="bff08-153">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="bff08-153">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="bff08-154">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="bff08-154">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="bff08-155">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="bff08-155">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="bff08-156">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="bff08-156">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="bff08-157">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="bff08-157">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="bff08-158">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="bff08-158">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bff08-159">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="bff08-159">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="bff08-160">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="bff08-160">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="bff08-161">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="bff08-161">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="bff08-162">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="bff08-162">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="bff08-163">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="bff08-163">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="bff08-164">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="bff08-164">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="bff08-165">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="bff08-165">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="bff08-166">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="bff08-166">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="bff08-167">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="bff08-167">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="bff08-168">ACR</span><span class="sxs-lookup"><span data-stu-id="bff08-168">ACR</span></span>

* <span data-ttu-id="bff08-169">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-169">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="bff08-170">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="bff08-170">Support SKU update for managed registries</span></span>
* <span data-ttu-id="bff08-171">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-171">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="bff08-172">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-172">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="bff08-173">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-173">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="bff08-174">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-174">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="bff08-175">ACS</span><span class="sxs-lookup"><span data-stu-id="bff08-175">ACS</span></span>

* <span data-ttu-id="bff08-176">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="bff08-176">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="bff08-177">AppService</span><span class="sxs-lookup"><span data-stu-id="bff08-177">Appservice</span></span>

* <span data-ttu-id="bff08-178">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="bff08-178">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="bff08-179">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="bff08-179">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="bff08-180">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="bff08-180">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="bff08-181">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="bff08-181">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="bff08-182">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="bff08-182">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="bff08-183">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="bff08-183">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="bff08-184">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="bff08-184">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="bff08-185">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="bff08-185">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="bff08-186">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="bff08-186">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="bff08-187">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="bff08-187">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="bff08-188">Batch</span><span class="sxs-lookup"><span data-stu-id="bff08-188">Batch</span></span>

* <span data-ttu-id="bff08-189">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="bff08-189">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="bff08-190">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="bff08-190">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="bff08-191">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-191">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="bff08-192">CDN</span><span class="sxs-lookup"><span data-stu-id="bff08-192">CDN</span></span>

* <span data-ttu-id="bff08-193">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="bff08-193">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="bff08-194">Cloud</span><span class="sxs-lookup"><span data-stu-id="bff08-194">Cloud</span></span>

* <span data-ttu-id="bff08-195">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="bff08-195">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="bff08-196">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="bff08-196">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="bff08-197">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="bff08-197">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="bff08-198">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="bff08-198">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="bff08-199">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="bff08-199">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bff08-200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bff08-200">CosmosDB</span></span>

* <span data-ttu-id="bff08-201">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="bff08-201">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="bff08-202">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-202">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bff08-203">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bff08-203">Data Lake Analytics</span></span>

* <span data-ttu-id="bff08-204">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-204">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="bff08-205">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-205">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="bff08-206">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-206">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bff08-207">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="bff08-207">Data Lake Store</span></span>

* <span data-ttu-id="bff08-208">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-208">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="bff08-209">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="bff08-209">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="bff08-210">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="bff08-210">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="bff08-211">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="bff08-211">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="bff08-212">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="bff08-212">Interactive</span></span>

* <span data-ttu-id="bff08-213">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="bff08-213">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="bff08-214">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="bff08-214">Increased test coverage</span></span>
* <span data-ttu-id="bff08-215">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="bff08-215">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="bff08-216">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="bff08-216">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="bff08-217">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="bff08-217">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="bff08-218">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="bff08-218">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="bff08-219">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="bff08-219">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bff08-220">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-220">Added `--progress` flag</span></span>
* <span data-ttu-id="bff08-221">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="bff08-221">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="bff08-222">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="bff08-222">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="bff08-223">IoT</span><span class="sxs-lookup"><span data-stu-id="bff08-223">IoT</span></span>

* <span data-ttu-id="bff08-224">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="bff08-224">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="bff08-225">(3934)</span><span class="sxs-lookup"><span data-stu-id="bff08-225">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="bff08-226">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="bff08-226">Key vault</span></span>

* <span data-ttu-id="bff08-227">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="bff08-227">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="bff08-228">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bff08-228">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="bff08-229">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bff08-229">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bff08-230">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bff08-230">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bff08-231">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bff08-231">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="bff08-232">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="bff08-232">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="bff08-233">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="bff08-233">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="bff08-234">(3307)</span><span class="sxs-lookup"><span data-stu-id="bff08-234">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="bff08-235">Labor</span><span class="sxs-lookup"><span data-stu-id="bff08-235">Lab</span></span>

* <span data-ttu-id="bff08-236">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-236">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="bff08-237">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-237">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="bff08-238">Überwachen</span><span class="sxs-lookup"><span data-stu-id="bff08-238">Monitor</span></span>

* <span data-ttu-id="bff08-239">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="bff08-239">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="bff08-240">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="bff08-240">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="bff08-241">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="bff08-241">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="bff08-242">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="bff08-242">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="bff08-243">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="bff08-243">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="bff08-244">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="bff08-244">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="bff08-245">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="bff08-245">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="bff08-246">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="bff08-246">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="bff08-247">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="bff08-247">`location` no longer required</span></span>
  * <span data-ttu-id="bff08-248">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="bff08-248">Add name and ID support for target</span></span>
  * <span data-ttu-id="bff08-249">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="bff08-249">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="bff08-250">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="bff08-250">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="bff08-251">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bff08-251">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="bff08-252">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="bff08-252">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="bff08-253">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="bff08-253">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="bff08-254">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-254">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="bff08-255">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="bff08-255">Network</span></span>

* <span data-ttu-id="bff08-256">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-256">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="bff08-257">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-257">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="bff08-258">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="bff08-258">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="bff08-259">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="bff08-259">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="bff08-260">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="bff08-260">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="bff08-261">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-261">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="bff08-262">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="bff08-262">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="bff08-263">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="bff08-263">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="bff08-264">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="bff08-264">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="bff08-265">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bff08-265">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="bff08-266">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-266">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="bff08-267">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-267">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="bff08-268">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="bff08-268">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="bff08-269">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-269">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="bff08-270">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-270">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="bff08-271">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="bff08-271">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="bff08-272">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-272">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="bff08-273">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="bff08-273">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="bff08-274">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-274">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="bff08-275">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="bff08-275">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="bff08-276">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="bff08-276">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="bff08-277">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="bff08-277">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="bff08-278">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="bff08-278">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="bff08-279">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="bff08-279">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="bff08-280">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="bff08-280">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="bff08-281">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="bff08-281">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="bff08-282">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="bff08-282">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="bff08-283">Profil</span><span class="sxs-lookup"><span data-stu-id="bff08-283">Profile</span></span>

* <span data-ttu-id="bff08-284">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="bff08-284">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="bff08-285">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="bff08-285">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="bff08-286">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="bff08-286">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="bff08-287">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-287">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="bff08-288">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="bff08-288">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="bff08-289">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bff08-289">RDBMS</span></span>

* <span data-ttu-id="bff08-290">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="bff08-290">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="bff08-291">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="bff08-291">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="bff08-292">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="bff08-292">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="bff08-293">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="bff08-293">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="bff08-294">Ressource</span><span class="sxs-lookup"><span data-stu-id="bff08-294">Resource</span></span>

* <span data-ttu-id="bff08-295">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="bff08-295">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="bff08-296">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="bff08-296">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="bff08-297">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="bff08-297">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="bff08-298">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="bff08-298">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="bff08-299">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="bff08-299">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="bff08-300">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="bff08-300">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="bff08-301">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="bff08-301">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="bff08-302">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-302">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="bff08-303">Rolle</span><span class="sxs-lookup"><span data-stu-id="bff08-303">Role</span></span>

* <span data-ttu-id="bff08-304">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="bff08-304">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="bff08-305">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="bff08-305">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="bff08-306">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="bff08-306">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="bff08-307">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="bff08-307">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="bff08-308">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-308">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bff08-309">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bff08-309">Service Fabric</span></span>
* <span data-ttu-id="bff08-310">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="bff08-310">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="bff08-311">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="bff08-311">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="bff08-312">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="bff08-312">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="bff08-313">SQL</span><span class="sxs-lookup"><span data-stu-id="bff08-313">SQL</span></span>

* <span data-ttu-id="bff08-314">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="bff08-314">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="bff08-315">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="bff08-315">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="bff08-316">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-316">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="bff08-317">Speicher</span><span class="sxs-lookup"><span data-stu-id="bff08-317">Storage</span></span>

* <span data-ttu-id="bff08-318">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="bff08-318">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="bff08-319">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="bff08-319">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="bff08-320">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="bff08-320">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="bff08-321">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="bff08-321">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="bff08-322">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="bff08-322">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="bff08-323">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="bff08-323">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="bff08-324">VM</span><span class="sxs-lookup"><span data-stu-id="bff08-324">VM</span></span>

* <span data-ttu-id="bff08-325">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="bff08-325">Support configuring nsg</span></span>
* <span data-ttu-id="bff08-326">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="bff08-326">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="bff08-327">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="bff08-327">Support managed service identities</span></span>
* <span data-ttu-id="bff08-328">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="bff08-328">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="bff08-329">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="bff08-329">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="bff08-330">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-330">May 10, 2017</span></span>

<span data-ttu-id="bff08-331">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="bff08-331">Version 2.0.6</span></span>

* <span data-ttu-id="bff08-332">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="bff08-332">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="bff08-333">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="bff08-333">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="bff08-334">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="bff08-334">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="bff08-335">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="bff08-335">Include Cognitive Services module.</span></span>
* <span data-ttu-id="bff08-336">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="bff08-336">Include Service Fabric module.</span></span>
* <span data-ttu-id="bff08-337">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="bff08-337">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="bff08-338">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="bff08-338">Add support for CDN commands.</span></span>
* <span data-ttu-id="bff08-339">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="bff08-339">Remove Container module.</span></span>
* <span data-ttu-id="bff08-340">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="bff08-340">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="bff08-341">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bff08-341">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="bff08-342">Core</span><span class="sxs-lookup"><span data-stu-id="bff08-342">Core</span></span>

* <span data-ttu-id="bff08-343">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="bff08-343">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="bff08-344">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="bff08-344">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="bff08-345">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="bff08-345">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="bff08-346">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="bff08-346">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="bff08-347">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="bff08-347">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="bff08-348">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="bff08-348">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="bff08-349">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="bff08-349">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="bff08-350">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="bff08-350">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="bff08-351">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="bff08-351">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="bff08-352">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="bff08-352">core: Improved performance</span></span>
* <span data-ttu-id="bff08-353">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="bff08-353">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="bff08-354">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="bff08-354">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="bff08-355">ACS</span><span class="sxs-lookup"><span data-stu-id="bff08-355">ACS</span></span>

* <span data-ttu-id="bff08-356">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bff08-356">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="bff08-357">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="bff08-357">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="bff08-358">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="bff08-358">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="bff08-359">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="bff08-359">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="bff08-360">AppService</span><span class="sxs-lookup"><span data-stu-id="bff08-360">AppService</span></span>

* <span data-ttu-id="bff08-361">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="bff08-361">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="bff08-362">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="bff08-362">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="bff08-363">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="bff08-363">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="bff08-364">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="bff08-364">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="bff08-365">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="bff08-365">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="bff08-366">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="bff08-366">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="bff08-367">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="bff08-367">support slot swap with preview</span></span>
* <span data-ttu-id="bff08-368">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="bff08-368">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="bff08-369">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="bff08-369">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bff08-370">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bff08-370">CosmosDB</span></span>

* <span data-ttu-id="bff08-371">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="bff08-371">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="bff08-372">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="bff08-372">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="bff08-373">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="bff08-373">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="bff08-374">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="bff08-374">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bff08-375">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bff08-375">Data Lake Analytics</span></span>

* <span data-ttu-id="bff08-376">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="bff08-376">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="bff08-377">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="bff08-377">Add support for new catalog item type: package.</span></span> <span data-ttu-id="bff08-378">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="bff08-378">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="bff08-379">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="bff08-379">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="bff08-380">Table</span><span class="sxs-lookup"><span data-stu-id="bff08-380">Table</span></span>
  * <span data-ttu-id="bff08-381">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="bff08-381">Table valued function</span></span>
  * <span data-ttu-id="bff08-382">Sicht</span><span class="sxs-lookup"><span data-stu-id="bff08-382">View</span></span>
  * <span data-ttu-id="bff08-383">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="bff08-383">Table Statistics.</span></span> <span data-ttu-id="bff08-384">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="bff08-384">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bff08-385">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bff08-385">Data Lake Store</span></span>

* <span data-ttu-id="bff08-386">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="bff08-386">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="bff08-387">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bff08-387">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="bff08-388">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="bff08-388">missed help for access show.</span></span> <span data-ttu-id="bff08-389">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="bff08-389">adding it.</span></span> <span data-ttu-id="bff08-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="bff08-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="bff08-391">Suchen</span><span class="sxs-lookup"><span data-stu-id="bff08-391">Find</span></span>

* <span data-ttu-id="bff08-392">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="bff08-392">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="bff08-393">KeyVault</span><span class="sxs-lookup"><span data-stu-id="bff08-393">KeyVault</span></span>

* <span data-ttu-id="bff08-394">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="bff08-394">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="bff08-395">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="bff08-395">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="bff08-396">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="bff08-396">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="bff08-397">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="bff08-397">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="bff08-398">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="bff08-398">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="bff08-399">Labor</span><span class="sxs-lookup"><span data-stu-id="bff08-399">Lab</span></span>

* <span data-ttu-id="bff08-400">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="bff08-400">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="bff08-401">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="bff08-401">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="bff08-402">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="bff08-402">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="bff08-403">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="bff08-403">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="bff08-404">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="bff08-404">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="bff08-405">Überwachen</span><span class="sxs-lookup"><span data-stu-id="bff08-405">Monitor</span></span>

* <span data-ttu-id="bff08-406">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="bff08-406">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="bff08-407">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="bff08-407">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="bff08-408">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="bff08-408">Network</span></span>

* <span data-ttu-id="bff08-409">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="bff08-409">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="bff08-410">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="bff08-410">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="bff08-411">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="bff08-411">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="bff08-412">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="bff08-412">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="bff08-413">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="bff08-413">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="bff08-414">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="bff08-414">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="bff08-415">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="bff08-415">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="bff08-416">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="bff08-416">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="bff08-417">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="bff08-417">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="bff08-418">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="bff08-418">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="bff08-419">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="bff08-419">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="bff08-420">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="bff08-420">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="bff08-421">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="bff08-421">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="bff08-422">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="bff08-422">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="bff08-423">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="bff08-423">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="bff08-424">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="bff08-424">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="bff08-425">Profil</span><span class="sxs-lookup"><span data-stu-id="bff08-425">Profile</span></span>

* <span data-ttu-id="bff08-426">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="bff08-426">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="bff08-427">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="bff08-427">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="bff08-428">Redis</span><span class="sxs-lookup"><span data-stu-id="bff08-428">Redis</span></span>

* <span data-ttu-id="bff08-429">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="bff08-429">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="bff08-430">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="bff08-430">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="bff08-431">Ressource</span><span class="sxs-lookup"><span data-stu-id="bff08-431">Resource</span></span>

* <span data-ttu-id="bff08-432">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="bff08-432">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="bff08-433">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="bff08-433">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="bff08-434">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="bff08-434">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="bff08-435">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="bff08-435">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="bff08-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="bff08-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="bff08-437">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="bff08-437">Add docs for az lock update.</span></span> <span data-ttu-id="bff08-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="bff08-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="bff08-439">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="bff08-439">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="bff08-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="bff08-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="bff08-441">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="bff08-441">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="bff08-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="bff08-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="bff08-443">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="bff08-443">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="bff08-444">Rolle</span><span class="sxs-lookup"><span data-stu-id="bff08-444">Role</span></span>

* <span data-ttu-id="bff08-445">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="bff08-445">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="bff08-446">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="bff08-446">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="bff08-447">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="bff08-447">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="bff08-448">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="bff08-448">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="bff08-449">SQL</span><span class="sxs-lookup"><span data-stu-id="bff08-449">SQL</span></span>

* <span data-ttu-id="bff08-450">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="bff08-450">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="bff08-451">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="bff08-451">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="bff08-452">Speicher</span><span class="sxs-lookup"><span data-stu-id="bff08-452">Storage</span></span>

* <span data-ttu-id="bff08-453">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="bff08-453">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="bff08-454">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="bff08-454">Add support for incremental blob copy</span></span>
* <span data-ttu-id="bff08-455">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="bff08-455">Add support for large block blob upload</span></span>
* <span data-ttu-id="bff08-456">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="bff08-456">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="bff08-457">VM</span><span class="sxs-lookup"><span data-stu-id="bff08-457">VM</span></span>

* <span data-ttu-id="bff08-458">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="bff08-458">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="bff08-459">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="bff08-459">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="bff08-460">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="bff08-460">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="bff08-461">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="bff08-461">az vm/vmss disk</span></span>
  3. <span data-ttu-id="bff08-462">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="bff08-462">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="bff08-463">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="bff08-463">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="bff08-464">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="bff08-464">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="bff08-465">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-465">April 3, 2017</span></span>

<span data-ttu-id="bff08-466">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="bff08-466">Version 2.0.2</span></span>

<span data-ttu-id="bff08-467">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="bff08-467">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="bff08-468">Core</span><span class="sxs-lookup"><span data-stu-id="bff08-468">Core</span></span>

* <span data-ttu-id="bff08-469">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="bff08-469">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="bff08-470">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="bff08-470">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="bff08-471">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="bff08-471">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="bff08-472">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bff08-472">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bff08-473">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="bff08-473">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="bff08-474">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="bff08-474">Add prompting for missing template parameters.</span></span> <span data-ttu-id="bff08-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="bff08-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="bff08-476">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="bff08-476">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="bff08-477">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="bff08-477">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="bff08-478">ACS</span><span class="sxs-lookup"><span data-stu-id="bff08-478">ACS</span></span>

* <span data-ttu-id="bff08-479">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="bff08-479">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="bff08-480">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="bff08-480">Add support for ssh key password prompting.</span></span> <span data-ttu-id="bff08-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="bff08-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="bff08-482">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="bff08-482">Add support for windows clusters.</span></span> <span data-ttu-id="bff08-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="bff08-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="bff08-484">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="bff08-484">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="bff08-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="bff08-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="bff08-486">AppService</span><span class="sxs-lookup"><span data-stu-id="bff08-486">AppService</span></span>

* <span data-ttu-id="bff08-487">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="bff08-487">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="bff08-488">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="bff08-488">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="bff08-489">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="bff08-489">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="bff08-490">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="bff08-490">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="bff08-491">DataLake</span><span class="sxs-lookup"><span data-stu-id="bff08-491">DataLake</span></span>

* <span data-ttu-id="bff08-492">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="bff08-492">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="bff08-493">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="bff08-493">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="bff08-494">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="bff08-494">DocuemntDB</span></span>

* <span data-ttu-id="bff08-495">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="bff08-495">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="bff08-496">VM</span><span class="sxs-lookup"><span data-stu-id="bff08-496">VM</span></span>

* <span data-ttu-id="bff08-497">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="bff08-497">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="bff08-498">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="bff08-498">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="bff08-499">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="bff08-499">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="bff08-500">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bff08-500">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bff08-501">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="bff08-501">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="bff08-502">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="bff08-502">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="bff08-503">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="bff08-503">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="bff08-504">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="bff08-504">February 27, 2017</span></span>

<span data-ttu-id="bff08-505">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="bff08-505">Version 2.0.0</span></span>

<span data-ttu-id="bff08-506">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="bff08-506">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="bff08-507">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="bff08-507">General availability applies to these command modules:</span></span>
- <span data-ttu-id="bff08-508">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="bff08-508">Container Service (acs)</span></span>
- <span data-ttu-id="bff08-509">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="bff08-509">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="bff08-510">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="bff08-510">Networking</span></span>
- <span data-ttu-id="bff08-511">Storage</span><span class="sxs-lookup"><span data-stu-id="bff08-511">Storage</span></span>

<span data-ttu-id="bff08-512">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bff08-512">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="bff08-513">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="bff08-513">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="bff08-514">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="bff08-514">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="bff08-515">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="bff08-515">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="bff08-516">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="bff08-516">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="bff08-517">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="bff08-517">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="bff08-518">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="bff08-518">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="bff08-519">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="bff08-519">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="bff08-520">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="bff08-520">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="bff08-521">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="bff08-521">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="bff08-522">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="bff08-522">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="bff08-523">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="bff08-523">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="bff08-524">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="bff08-524">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="bff08-525">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="bff08-525">Provide feedback from the command line with the `az feedback` command.</span></span>

