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
ms.openlocfilehash: fd5d82e34089a9a884c25c9a5620526f9d30577a
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="67cb4-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="67cb4-103">Azure CLI 2.0 release notes</span></span>

## <a name="april-10-2018"></a><span data-ttu-id="67cb4-104">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-104">April 10, 2018</span></span>

<span data-ttu-id="67cb4-105">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="67cb4-105">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-106">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-106">ACR</span></span>

* <span data-ttu-id="67cb4-107">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="67cb4-107">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-108">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-108">ACS</span></span>

* <span data-ttu-id="67cb4-109">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-109">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-110">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-110">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="67cb4-112">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-112">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="67cb4-113">Batch AI</span><span class="sxs-lookup"><span data-stu-id="67cb4-113">BatchAI</span></span>

* <span data-ttu-id="67cb4-114">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-114">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="67cb4-115">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="67cb4-115">Job level mounting</span></span>
 - <span data-ttu-id="67cb4-116">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="67cb4-116">Environment variables with secret values</span></span>
 - <span data-ttu-id="67cb4-117">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="67cb4-117">Performance counters settings</span></span>
 - <span data-ttu-id="67cb4-118">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="67cb4-118">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="67cb4-119">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="67cb4-119">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="67cb4-120">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="67cb4-120">Usage and limits reporting</span></span>
 - <span data-ttu-id="67cb4-121">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="67cb4-121">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="67cb4-122">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="67cb4-122">Support for custom images</span></span>
 - <span data-ttu-id="67cb4-123">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-123">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="67cb4-124">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="67cb4-124">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="67cb4-125">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="67cb4-125">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="67cb4-126">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="67cb4-126">National clouds are supported</span></span>
* <span data-ttu-id="67cb4-127">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-127">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="67cb4-128">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="67cb4-128">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="67cb4-129">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-129">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="67cb4-130">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="67cb4-130">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="67cb4-131">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="67cb4-131">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="67cb4-132">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="67cb4-132">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="67cb4-133">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="67cb4-133">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="67cb4-134">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-134">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="67cb4-135">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="67cb4-135">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="67cb4-136">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-136">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="67cb4-137">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="67cb4-137">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="67cb4-138">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-138">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="67cb4-139">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="67cb4-139">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="67cb4-140">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="67cb4-140">Billing</span></span>

* <span data-ttu-id="67cb4-141">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-141">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="67cb4-142">Nutzung</span><span class="sxs-lookup"><span data-stu-id="67cb4-142">Consumption</span></span>

* <span data-ttu-id="67cb4-143">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-143">Added `marketplace` commands</span></span>
* <span data-ttu-id="67cb4-144">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-144">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="67cb4-145">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-145">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="67cb4-146">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-146">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="67cb4-147">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-147">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="67cb4-148">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-148">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-149">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-149">Container</span></span>

* <span data-ttu-id="67cb4-150">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-150">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="67cb4-151">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="67cb4-151">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-152">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-152">Extension</span></span>

* <span data-ttu-id="67cb4-153">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-153">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-154">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-154">Interactive</span></span>

* <span data-ttu-id="67cb4-155">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="67cb4-155">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="67cb4-156">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-156">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="67cb4-157">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-157">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-158">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-158">Network</span></span>

* <span data-ttu-id="67cb4-159">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="67cb4-159">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="67cb4-160">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-160">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="67cb4-161">#4910</span><span class="sxs-lookup"><span data-stu-id="67cb4-161">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="67cb4-162">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-162">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="67cb4-163">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-163">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="67cb4-164">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-164">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="67cb4-165">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-165">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="67cb4-166">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-166">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-167">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-167">Profile</span></span>

* <span data-ttu-id="67cb4-168">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-168">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="67cb4-169">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-169">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="67cb4-170">RDBMS</span><span class="sxs-lookup"><span data-stu-id="67cb4-170">RDBMS</span></span>

* <span data-ttu-id="67cb4-171">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-171">Added `georestore` command</span></span>
* <span data-ttu-id="67cb4-172">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-172">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-173">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-173">Resource</span></span>

* <span data-ttu-id="67cb4-174">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-174">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="67cb4-175">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-175">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-176">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-176">SQL</span></span>

* <span data-ttu-id="67cb4-177">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-177">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-178">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-178">Storage</span></span>

* <span data-ttu-id="67cb4-179">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-179">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-180">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-180">VM</span></span>

* <span data-ttu-id="67cb4-181">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-181">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="67cb4-182">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-182">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="67cb4-184">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-184">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="67cb4-185">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="67cb4-185">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="67cb4-186">#5718</span><span class="sxs-lookup"><span data-stu-id="67cb4-186">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="67cb4-187">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="67cb4-187">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="67cb4-188">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-188">March 27, 2018</span></span>

<span data-ttu-id="67cb4-189">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="67cb4-189">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-190">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-190">Core</span></span>

* <span data-ttu-id="67cb4-191">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="67cb4-191">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-192">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-192">ACS</span></span>

* <span data-ttu-id="67cb4-193">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="67cb4-193">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-194">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-194">Appservice</span></span>

* <span data-ttu-id="67cb4-195">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-195">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="67cb4-196">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-196">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="67cb4-197">Sicherung</span><span class="sxs-lookup"><span data-stu-id="67cb4-197">Backup</span></span>

* <span data-ttu-id="67cb4-198">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-198">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="67cb4-199">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="67cb4-199">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="67cb4-200">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="67cb4-200">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="67cb4-201">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="67cb4-201">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-202">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-202">Container</span></span>

* <span data-ttu-id="67cb4-203">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-203">Added `container exec` command.</span></span> <span data-ttu-id="67cb4-204">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="67cb4-204">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="67cb4-205">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="67cb4-205">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-206">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-206">Extension</span></span>

* <span data-ttu-id="67cb4-207">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="67cb4-207">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="67cb4-208">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="67cb4-208">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="67cb4-209">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="67cb4-209">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-210">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-210">Interactive</span></span>

* <span data-ttu-id="67cb4-211">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="67cb4-211">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="67cb4-212">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-212">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="67cb4-213">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67cb4-213">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="67cb4-214">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="67cb4-214">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="67cb4-215">Labor</span><span class="sxs-lookup"><span data-stu-id="67cb4-215">Lab</span></span>

* <span data-ttu-id="67cb4-216">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-216">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-217">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-217">Monitor</span></span>

* <span data-ttu-id="67cb4-218">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="67cb4-218">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="67cb4-219">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="67cb4-219">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="67cb4-220">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="67cb4-220">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-221">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-221">Network</span></span>

* <span data-ttu-id="67cb4-222">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-222">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-223">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-223">Profile</span></span>

* <span data-ttu-id="67cb4-224">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-224">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="67cb4-225">RDBMS</span><span class="sxs-lookup"><span data-stu-id="67cb4-225">RDBMS</span></span>

* <span data-ttu-id="67cb4-226">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-226">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-227">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-227">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="67cb4-229">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-229">Role</span></span>

* <span data-ttu-id="67cb4-230">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-230">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="67cb4-231">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="67cb4-231">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="67cb4-232">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-232">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="67cb4-233">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-233">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="67cb4-234">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-234">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-235">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-235">Storage</span></span>

* <span data-ttu-id="67cb4-236">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-236">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="67cb4-237">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="67cb4-237">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-238">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-238">VM</span></span>

* <span data-ttu-id="67cb4-239">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-239">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="67cb4-240">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-240">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="67cb4-241">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="67cb4-241">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="67cb4-242">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="67cb4-242">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="67cb4-243">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-243">March 13, 2018</span></span>

<span data-ttu-id="67cb4-244">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="67cb4-244">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-245">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-245">ACR</span></span>

* <span data-ttu-id="67cb4-246">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-246">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="67cb4-247">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-247">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="67cb4-248">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-248">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-249">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-249">ACS</span></span>

* <span data-ttu-id="67cb4-250">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-250">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="67cb4-251">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-251">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="67cb4-252">Advisor</span><span class="sxs-lookup"><span data-stu-id="67cb4-252">Advisor</span></span>

* <span data-ttu-id="67cb4-253">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-253">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="67cb4-254">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-254">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="67cb4-255">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-255">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="67cb4-256">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-256">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="67cb4-257">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-257">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-258">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-258">Appservice</span></span>

* <span data-ttu-id="67cb4-259">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-259">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="67cb4-260">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-260">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="67cb4-261">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="67cb4-261">Eventhubs</span></span>

* <span data-ttu-id="67cb4-262">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-262">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-263">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-263">Extension</span></span>

* <span data-ttu-id="67cb4-264">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="67cb4-264">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-265">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-265">Interactive</span></span>

* <span data-ttu-id="67cb4-266">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="67cb4-266">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="67cb4-267">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="67cb4-267">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="67cb4-268">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="67cb4-268">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="67cb4-269">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-269">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-270">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-270">Monitor</span></span>

* <span data-ttu-id="67cb4-271">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-271">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="67cb4-272">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-272">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="67cb4-273">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-273">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="67cb4-274">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-274">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-275">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-275">Network</span></span>

* <span data-ttu-id="67cb4-276">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-276">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="67cb4-277">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="67cb4-277">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="67cb4-278">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-278">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="67cb4-279">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-279">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-280">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-280">Profile</span></span>

* <span data-ttu-id="67cb4-281">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-281">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="67cb4-282">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-282">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="67cb4-283">RDBMS</span><span class="sxs-lookup"><span data-stu-id="67cb4-283">RDBMS</span></span>

* <span data-ttu-id="67cb4-284">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-284">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="67cb4-285">SERVICE BUS</span><span class="sxs-lookup"><span data-stu-id="67cb4-285">Service Bus</span></span>

* <span data-ttu-id="67cb4-286">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-286">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-287">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-287">Storage</span></span>

* <span data-ttu-id="67cb4-288">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="67cb4-288">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="67cb4-289">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="67cb4-289">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-290">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-290">VM</span></span>

* <span data-ttu-id="67cb4-291">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="67cb4-291">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="67cb4-292">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-292">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="67cb4-293">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-293">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="67cb4-294">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-294">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="67cb4-295">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-295">February 27, 2018</span></span>

<span data-ttu-id="67cb4-296">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="67cb4-296">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-297">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-297">Core</span></span>

* <span data-ttu-id="67cb4-298">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-298">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="67cb4-299">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-299">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="67cb4-300">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-300">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-301">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-301">ACS</span></span>

* <span data-ttu-id="67cb4-302">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-302">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="67cb4-303">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="67cb4-303">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="67cb4-304">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-304">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="67cb4-305">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-305">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-306">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-306">Appservice</span></span>

* <span data-ttu-id="67cb4-307">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="67cb4-307">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="67cb4-308">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="67cb4-308">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="67cb4-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="67cb4-309">Cognitive Services</span></span>

* <span data-ttu-id="67cb4-310">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-310">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="67cb4-311">Nutzung</span><span class="sxs-lookup"><span data-stu-id="67cb4-311">Consumption</span></span>

* <span data-ttu-id="67cb4-312">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-312">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="67cb4-313">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-313">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-314">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-314">Container</span></span>

* <span data-ttu-id="67cb4-315">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="67cb4-315">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-316">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-316">Network</span></span>

* <span data-ttu-id="67cb4-317">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="67cb4-317">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-318">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-318">Resource</span></span>

* <span data-ttu-id="67cb4-319">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="67cb4-319">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-320">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-320">Role</span></span>

* <span data-ttu-id="67cb4-321">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-321">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-322">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-322">SQL</span></span>

* <span data-ttu-id="67cb4-323">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="67cb4-323">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-324">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-324">Storage</span></span>

* <span data-ttu-id="67cb4-325">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-325">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-326">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-326">VM</span></span>

* <span data-ttu-id="67cb4-327">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-327">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="67cb4-328">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-328">February 13, 2018</span></span>

<span data-ttu-id="67cb4-329">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="67cb4-329">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-330">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-330">Core</span></span>

* <span data-ttu-id="67cb4-331">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-331">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-332">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-332">ACS</span></span>

* <span data-ttu-id="67cb4-333">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-333">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="67cb4-334">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-334">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="67cb4-335">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-335">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="67cb4-336">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-336">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="67cb4-337">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-337">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="67cb4-338">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-338">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="67cb4-339">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="67cb4-339">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="67cb4-340">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="67cb4-340">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-341">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-341">Appservice</span></span>

* <span data-ttu-id="67cb4-342">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="67cb4-342">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="67cb4-343">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-343">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="67cb4-344">CDN</span><span class="sxs-lookup"><span data-stu-id="67cb4-344">CDN</span></span>

* <span data-ttu-id="67cb4-345">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-345">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-346">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-346">Container</span></span>

* <span data-ttu-id="67cb4-347">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-347">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="67cb4-348">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-348">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67cb4-349">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67cb4-349">CosmosDB</span></span>

* <span data-ttu-id="67cb4-350">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-350">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-351">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-351">Extension</span></span>

* <span data-ttu-id="67cb4-352">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-352">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="67cb4-353">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-353">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="67cb4-354">Feedback</span><span class="sxs-lookup"><span data-stu-id="67cb4-354">Feedback</span></span>

* <span data-ttu-id="67cb4-355">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-355">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-356">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-356">Interactive</span></span>

* <span data-ttu-id="67cb4-357">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-357">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="67cb4-358">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-358">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="67cb4-359">IoT</span><span class="sxs-lookup"><span data-stu-id="67cb4-359">IoT</span></span>

* <span data-ttu-id="67cb4-360">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="67cb4-360">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="67cb4-361">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="67cb4-361">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="67cb4-362">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-362">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="67cb4-363">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-363">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-364">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-364">Monitor</span></span>

* <span data-ttu-id="67cb4-365">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-365">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-366">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-366">Network</span></span>

* <span data-ttu-id="67cb4-367">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="67cb4-367">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="67cb4-368">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-368">Profile</span></span>

* <span data-ttu-id="67cb4-369">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="67cb4-369">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-370">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-370">Resource</span></span>

* <span data-ttu-id="67cb4-371">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-371">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-372">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-372">Role</span></span>

* <span data-ttu-id="67cb4-373">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-373">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-374">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-374">SQL</span></span>

* <span data-ttu-id="67cb4-375">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-375">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="67cb4-376">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-376">Added `sql db rename`</span></span>
* <span data-ttu-id="67cb4-377">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-377">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-378">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-378">Storage</span></span>

* <span data-ttu-id="67cb4-379">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-379">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-380">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-380">VM</span></span>

* <span data-ttu-id="67cb4-381">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-381">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="67cb4-382">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-382">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="67cb4-383">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="67cb4-383">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="67cb4-384">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-384">January 31, 2018</span></span>

<span data-ttu-id="67cb4-385">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="67cb4-385">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-386">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-386">Core</span></span>

* <span data-ttu-id="67cb4-387">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-387">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="67cb4-388">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-388">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="67cb4-389">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="67cb4-389">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="67cb4-390">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="67cb4-390">Use `--verbose` to see</span></span>
* <span data-ttu-id="67cb4-391">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-391">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-392">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-392">ACS</span></span>

* <span data-ttu-id="67cb4-393">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="67cb4-393">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="67cb4-394">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-394">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-395">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-395">Appservice</span></span>

* <span data-ttu-id="67cb4-396">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="67cb4-396">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="67cb4-397">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-397">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="67cb4-398">CDN</span><span class="sxs-lookup"><span data-stu-id="67cb4-398">CDN</span></span>

* <span data-ttu-id="67cb4-399">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-399">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67cb4-400">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67cb4-400">CosmosDB</span></span>

* <span data-ttu-id="67cb4-401">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-401">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-402">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-402">Interactive</span></span>

* <span data-ttu-id="67cb4-403">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-403">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-404">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-404">Network</span></span>

* <span data-ttu-id="67cb4-405">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-405">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="67cb4-406">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="67cb4-406">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="67cb4-407">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-407">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="67cb4-408">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-408">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="67cb4-409">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-409">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="67cb4-410">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="67cb4-410">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="67cb4-411">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-411">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="67cb4-412">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-412">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="67cb4-413">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-413">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="67cb4-414">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="67cb4-414">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-415">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-415">Profile</span></span>

* <span data-ttu-id="67cb4-416">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-416">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-417">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-417">Resource</span></span>

* <span data-ttu-id="67cb4-418">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="67cb4-418">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-419">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-419">Storage</span></span>

* <span data-ttu-id="67cb4-420">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-420">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="67cb4-421">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-421">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="67cb4-422">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="67cb4-422">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="67cb4-423">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-423">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="67cb4-424">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="67cb4-424">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-425">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-425">VM</span></span>

* <span data-ttu-id="67cb4-426">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-426">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="67cb4-427">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="67cb4-427">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="67cb4-428">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-428">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="67cb4-429">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-429">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="67cb4-430">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="67cb4-430">January 17, 2018</span></span>

<span data-ttu-id="67cb4-431">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="67cb4-431">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-432">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-432">ACR</span></span>

* <span data-ttu-id="67cb4-433">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-433">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="67cb4-434">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="67cb4-434">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-435">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-435">ACS</span></span>

* <span data-ttu-id="67cb4-436">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-436">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="67cb4-437">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-437">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-438">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-438">Appservice</span></span>

* <span data-ttu-id="67cb4-439">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="67cb4-439">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="67cb4-440">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-440">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="67cb4-441">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-441">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="67cb4-442">Sicherung</span><span class="sxs-lookup"><span data-stu-id="67cb4-442">Backup</span></span>

* <span data-ttu-id="67cb4-443">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="67cb4-443">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="67cb4-444">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-444">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="67cb4-445">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="67cb4-445">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="67cb4-446">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="67cb4-446">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="67cb4-447">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="67cb4-447">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="67cb4-448">Batch</span><span class="sxs-lookup"><span data-stu-id="67cb4-448">Batch</span></span>

* <span data-ttu-id="67cb4-449">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="67cb4-449">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="67cb4-450">Cloud</span><span class="sxs-lookup"><span data-stu-id="67cb4-450">Cloud</span></span>

* <span data-ttu-id="67cb4-451">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-451">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="67cb4-452">Nutzung</span><span class="sxs-lookup"><span data-stu-id="67cb4-452">Consumption</span></span>

* <span data-ttu-id="67cb4-453">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="67cb4-453">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="67cb4-454">Event Grid</span><span class="sxs-lookup"><span data-stu-id="67cb4-454">Event Grid</span></span>

* <span data-ttu-id="67cb4-455">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="67cb4-455">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="67cb4-456">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="67cb4-456">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="67cb4-457">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-457">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="67cb4-458">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="67cb4-458">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="67cb4-459">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-459">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="67cb4-460">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-460">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="67cb4-461">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-461">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="67cb4-462">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-462">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-463">Interactive</span><span class="sxs-lookup"><span data-stu-id="67cb4-463">Interactive</span></span>

* <span data-ttu-id="67cb4-464">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="67cb4-464">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="67cb4-465">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-465">Fixed errors on startup</span></span>
* <span data-ttu-id="67cb4-466">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="67cb4-466">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="67cb4-467">IoT</span><span class="sxs-lookup"><span data-stu-id="67cb4-467">IoT</span></span>

* <span data-ttu-id="67cb4-468">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-468">Added support for device provisioning service</span></span>
* <span data-ttu-id="67cb4-469">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-469">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="67cb4-470">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="67cb4-470">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-471">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-471">Monitor</span></span>

* <span data-ttu-id="67cb4-472">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-472">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="67cb4-473">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67cb4-473">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="67cb4-474">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-474">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-475">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-475">Network</span></span>

* <span data-ttu-id="67cb4-476">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="67cb4-476">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="67cb4-477">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-477">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-478">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-478">Profile</span></span>

* <span data-ttu-id="67cb4-479">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-479">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-480">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-480">Role</span></span>

* <span data-ttu-id="67cb4-481">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="67cb4-481">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="67cb4-482">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67cb4-482">Service Fabric</span></span>

* <span data-ttu-id="67cb4-483">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-483">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="67cb4-484">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-484">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-485">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-485">VM</span></span>

* <span data-ttu-id="67cb4-486">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="67cb4-486">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="67cb4-487">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-487">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="67cb4-488">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="67cb4-488">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="67cb4-489">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-489">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="67cb4-490">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-490">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="67cb4-491">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-491">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="67cb4-492">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-492">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="67cb4-493">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-493">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="67cb4-494">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-494">December 19, 2017</span></span>

<span data-ttu-id="67cb4-495">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="67cb4-495">Version 2.0.23</span></span>

* <span data-ttu-id="67cb4-496">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-496">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-497">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-497">Container</span></span>

* <span data-ttu-id="67cb4-498">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-498">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-499">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-499">Network</span></span>

* <span data-ttu-id="67cb4-500">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-500">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="67cb4-501">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-501">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-502">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-502">Storage</span></span>

* <span data-ttu-id="67cb4-503">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-503">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-504">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-504">VM</span></span>

* <span data-ttu-id="67cb4-505">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-505">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="67cb4-506">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-506">December 5, 2017</span></span>

<span data-ttu-id="67cb4-507">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="67cb4-507">Version 2.0.22</span></span>

* <span data-ttu-id="67cb4-508">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-508">Removed `az component` commands.</span></span> <span data-ttu-id="67cb4-509">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="67cb4-509">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-510">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-510">Core</span></span>
* <span data-ttu-id="67cb4-511">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="67cb4-511">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="67cb4-512">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-512">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-513">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-513">ACS</span></span>

* <span data-ttu-id="67cb4-514">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-514">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="67cb4-515">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="67cb4-515">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="67cb4-516">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="67cb4-516">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="67cb4-517">Advisor</span><span class="sxs-lookup"><span data-stu-id="67cb4-517">Advisor</span></span>

* <span data-ttu-id="67cb4-518">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-518">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-519">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-519">Appservice</span></span>

* <span data-ttu-id="67cb4-520">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="67cb4-520">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="67cb4-521">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="67cb4-521">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="67cb4-522">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-522">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="67cb4-523">Nutzung</span><span class="sxs-lookup"><span data-stu-id="67cb4-523">Consumption</span></span>

* <span data-ttu-id="67cb4-524">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-524">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-525">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-525">Container</span></span>

* <span data-ttu-id="67cb4-526">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="67cb4-526">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-527">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-527">Monitor</span></span>

* <span data-ttu-id="67cb4-528">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-528">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-529">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-529">Resource</span></span>

* <span data-ttu-id="67cb4-530">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-530">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-531">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-531">Role</span></span>

* <span data-ttu-id="67cb4-532">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-532">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="67cb4-533">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-533">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="67cb4-534">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="67cb4-534">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-535">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-535">SQL</span></span>

* <span data-ttu-id="67cb4-536">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-536">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="67cb4-537">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-537">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-538">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-538">VM</span></span>

* <span data-ttu-id="67cb4-539">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-539">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="67cb4-540">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-540">November 14, 2017</span></span>

<span data-ttu-id="67cb4-541">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="67cb4-541">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-542">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-542">ACR</span></span>

* <span data-ttu-id="67cb4-543">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-543">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="67cb4-544">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-544">ACS</span></span>

* <span data-ttu-id="67cb4-545">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-545">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="67cb4-546">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="67cb4-546">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="67cb4-547">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="67cb4-547">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="67cb4-548">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-548">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="67cb4-549">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-549">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-550">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-550">Appservice</span></span>

* <span data-ttu-id="67cb4-551">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-551">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="67cb4-552">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-552">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="67cb4-553">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-553">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="67cb4-554">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-554">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="67cb4-555">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-555">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="67cb4-556">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="67cb4-556">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="67cb4-557">Batch</span><span class="sxs-lookup"><span data-stu-id="67cb4-557">Batch</span></span>

* <span data-ttu-id="67cb4-558">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="67cb4-558">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="67cb4-559">BatchAI</span><span class="sxs-lookup"><span data-stu-id="67cb4-559">Batchai</span></span>

* <span data-ttu-id="67cb4-560">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-560">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="67cb4-561">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-561">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="67cb4-562">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-562">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="67cb4-563">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-563">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="67cb4-564">Cloud</span><span class="sxs-lookup"><span data-stu-id="67cb4-564">Cloud</span></span>

* <span data-ttu-id="67cb4-565">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="67cb4-565">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-566">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-566">Container</span></span>

* <span data-ttu-id="67cb4-567">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-567">Added support to open multiple ports</span></span>
* <span data-ttu-id="67cb4-568">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-568">Added container group restart policy</span></span>
* <span data-ttu-id="67cb4-569">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-569">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="67cb4-570">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-570">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67cb4-571">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67cb4-571">Data Lake Analytics</span></span>

* <span data-ttu-id="67cb4-572">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="67cb4-572">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67cb4-573">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-573">Data Lake Store</span></span>

* <span data-ttu-id="67cb4-574">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="67cb4-574">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-575">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-575">Extension</span></span>

* <span data-ttu-id="67cb4-576">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-576">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="67cb4-577">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67cb4-577">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="67cb4-578">IoT</span><span class="sxs-lookup"><span data-stu-id="67cb4-578">IoT</span></span>

* <span data-ttu-id="67cb4-579">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-579">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-580">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-580">Monitor</span></span>

* <span data-ttu-id="67cb4-581">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-581">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-582">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-582">Network</span></span>

* <span data-ttu-id="67cb4-583">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-583">Added support for CAA DNS records</span></span>
* <span data-ttu-id="67cb4-584">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="67cb4-584">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="67cb4-585">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="67cb4-585">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="67cb4-586">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-586">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="67cb4-587">Reservations</span><span class="sxs-lookup"><span data-stu-id="67cb4-587">Reservations</span></span>

* <span data-ttu-id="67cb4-588">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67cb4-588">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-589">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-589">Resource</span></span>

* <span data-ttu-id="67cb4-590">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-590">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-591">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-591">SQL</span></span>

* <span data-ttu-id="67cb4-592">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-592">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-593">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-593">Storage</span></span>

* <span data-ttu-id="67cb4-594">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-594">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="67cb4-595">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="67cb4-595">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="67cb4-596">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="67cb4-596">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="67cb4-597">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-597">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="67cb4-598">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-598">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="67cb4-599">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-599">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="67cb4-600">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-600">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-601">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-601">VM</span></span>

* <span data-ttu-id="67cb4-602">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="67cb4-602">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="67cb4-603">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-603">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="67cb4-604">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="67cb4-604">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="67cb4-605">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-605">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="67cb4-606">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-606">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="67cb4-607">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-607">October 24, 2017</span></span>

<span data-ttu-id="67cb4-608">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="67cb4-608">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-609">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-609">Core</span></span>

* <span data-ttu-id="67cb4-610">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="67cb4-610">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-611">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-611">ACR</span></span>

* <span data-ttu-id="67cb4-612">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="67cb4-612">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="67cb4-613">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="67cb4-613">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="67cb4-614">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-614">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-615">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-615">ACS</span></span>

* <span data-ttu-id="67cb4-616">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-616">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="67cb4-617">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-617">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-618">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-618">Appservice</span></span>

* <span data-ttu-id="67cb4-619">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="67cb4-619">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="67cb4-620">Komponente</span><span class="sxs-lookup"><span data-stu-id="67cb4-620">Component</span></span>

* <span data-ttu-id="67cb4-621">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-621">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-622">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-622">Monitor</span></span>

* <span data-ttu-id="67cb4-623">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-623">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-624">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-624">Resource</span></span>

* <span data-ttu-id="67cb4-625">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-625">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="67cb4-626">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="67cb4-626">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-627">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-627">VM</span></span>

* <span data-ttu-id="67cb4-628">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-628">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="67cb4-629">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-629">October 9, 2017</span></span>

<span data-ttu-id="67cb4-630">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="67cb4-630">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-631">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-631">Core</span></span>

* <span data-ttu-id="67cb4-632">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-632">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-633">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-633">Appservice</span></span>

* <span data-ttu-id="67cb4-634">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-634">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="67cb4-635">Batch</span><span class="sxs-lookup"><span data-stu-id="67cb4-635">Batch</span></span>

* <span data-ttu-id="67cb4-636">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="67cb4-636">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="67cb4-637">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-637">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="67cb4-638">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-638">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="67cb4-639">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-639">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="67cb4-640">BatchAI</span><span class="sxs-lookup"><span data-stu-id="67cb4-640">Batchai</span></span>

* <span data-ttu-id="67cb4-641">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-641">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="67cb4-642">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67cb4-642">Keyvault</span></span>

* <span data-ttu-id="67cb4-643">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="67cb4-643">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="67cb4-644">(#4448)</span><span class="sxs-lookup"><span data-stu-id="67cb4-644">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="67cb4-645">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-645">Network</span></span>

* <span data-ttu-id="67cb4-646">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="67cb4-646">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="67cb4-647">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-647">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-648">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-648">Resource</span></span>

* <span data-ttu-id="67cb4-649">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-649">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="67cb4-650">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-650">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="67cb4-651">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-651">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="67cb4-652">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-652">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-653">Sql</span><span class="sxs-lookup"><span data-stu-id="67cb4-653">Sql</span></span>

* <span data-ttu-id="67cb4-654">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-654">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="67cb4-655">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-655">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="67cb4-656">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-656">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-657">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-657">Storage</span></span>

* <span data-ttu-id="67cb4-658">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-658">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-659">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-659">Vm</span></span>

* <span data-ttu-id="67cb4-660">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="67cb4-660">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="67cb4-661">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-661">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="67cb4-662">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-662">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="67cb4-663">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-663">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="67cb4-664">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-664">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="67cb4-665">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-665">September 22, 2017</span></span>

<span data-ttu-id="67cb4-666">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="67cb4-666">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-667">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-667">Resource</span></span>

* <span data-ttu-id="67cb4-668">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-668">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="67cb4-669">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-669">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="67cb4-670">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-670">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="67cb4-671">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="67cb4-671">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-672">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-672">Network</span></span>

* <span data-ttu-id="67cb4-673">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-673">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="67cb4-674">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-674">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="67cb4-675">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-675">Added `asg` application security group commands</span></span>
* <span data-ttu-id="67cb4-676">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-676">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="67cb4-677">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-677">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="67cb4-678">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-678">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="67cb4-679">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-679">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-680">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-680">Storage</span></span>

* <span data-ttu-id="67cb4-681">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67cb4-681">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="67cb4-682">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="67cb4-682">Eventgrid</span></span>

* <span data-ttu-id="67cb4-683">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-683">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-684">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-684">SQL</span></span>

* <span data-ttu-id="67cb4-685">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="67cb4-685">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="67cb4-686">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67cb4-686">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="67cb4-687">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-687">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="67cb4-688">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67cb4-688">Keyvault</span></span>

* <span data-ttu-id="67cb4-689">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-689">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-690">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-690">VM</span></span>

* <span data-ttu-id="67cb4-691">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-691">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="67cb4-692">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67cb4-692">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="67cb4-693">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-693">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="67cb4-694">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-694">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="67cb4-695">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-695">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="67cb4-696">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-696">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-697">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-697">ACS</span></span>

* <span data-ttu-id="67cb4-698">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-698">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-699">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-699">Appservice</span></span>

* <span data-ttu-id="67cb4-700">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="67cb4-700">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="67cb4-701">Sicherung</span><span class="sxs-lookup"><span data-stu-id="67cb4-701">Backup</span></span>

* <span data-ttu-id="67cb4-702">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67cb4-702">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="67cb4-703">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-703">September 11, 2017</span></span>

<span data-ttu-id="67cb4-704">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="67cb4-704">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="67cb4-705">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-705">Core</span></span>

* <span data-ttu-id="67cb4-706">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="67cb4-706">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="67cb4-707">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="67cb4-707">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-708">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-708">Acs</span></span>

* <span data-ttu-id="67cb4-709">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-709">Added `acs list-locations` command</span></span>
* <span data-ttu-id="67cb4-710">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-710">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-711">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-711">Appservice</span></span>

* <span data-ttu-id="67cb4-712">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="67cb4-712">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="67cb4-713">CDN</span><span class="sxs-lookup"><span data-stu-id="67cb4-713">CDN</span></span>

* <span data-ttu-id="67cb4-714">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="67cb4-714">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="67cb4-715">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67cb4-715">Extension</span></span>

* <span data-ttu-id="67cb4-716">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-716">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="67cb4-717">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67cb4-717">Keyvault</span></span>

* <span data-ttu-id="67cb4-718">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="67cb4-718">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-719">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-719">Network</span></span>

* <span data-ttu-id="67cb4-720">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-720">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="67cb4-721">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-721">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="67cb4-722">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-722">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="67cb4-723">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-723">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="67cb4-724">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-724">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-725">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-725">Resource</span></span>

* <span data-ttu-id="67cb4-726">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="67cb4-726">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="67cb4-727">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="67cb4-727">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="67cb4-728">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="67cb4-728">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="67cb4-729">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-729">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-730">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-730">SQL</span></span>

* <span data-ttu-id="67cb4-731">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-731">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-732">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-732">VM</span></span>

* <span data-ttu-id="67cb4-733">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-733">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="67cb4-734">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="67cb4-734">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="67cb4-735">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-735">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="67cb4-736">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="67cb4-736">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="67cb4-737">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="67cb4-737">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="67cb4-738">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-738">August 31, 2017</span></span>

<span data-ttu-id="67cb4-739">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="67cb4-739">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="67cb4-740">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67cb4-740">Keyvault</span></span>

* <span data-ttu-id="67cb4-741">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="67cb4-741">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="67cb4-742">Sf</span><span class="sxs-lookup"><span data-stu-id="67cb4-742">Sf</span></span>

* <span data-ttu-id="67cb4-743">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-743">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-744">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-744">Storage</span></span>

* <span data-ttu-id="67cb4-745">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="67cb4-745">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="67cb4-746">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="67cb4-746">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="67cb4-747">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-747">August 28, 2017</span></span>

<span data-ttu-id="67cb4-748">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="67cb4-748">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="67cb4-749">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="67cb4-749">CLI</span></span>

* <span data-ttu-id="67cb4-750">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-750">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-751">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-751">ACS</span></span>

* <span data-ttu-id="67cb4-752">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-752">Corrected preview regions</span></span>
* <span data-ttu-id="67cb4-753">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-753">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="67cb4-754">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-754">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-755">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-755">Appservice</span></span>

* <span data-ttu-id="67cb4-756">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-756">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="67cb4-757">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-757">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="67cb4-758">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-758">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="67cb4-759">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="67cb4-759">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="67cb4-760">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-760">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="67cb4-761">IoT</span><span class="sxs-lookup"><span data-stu-id="67cb4-761">IoT</span></span>

* <span data-ttu-id="67cb4-762">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="67cb4-762">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-763">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-763">Network</span></span>

* <span data-ttu-id="67cb4-764">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-764">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="67cb4-765">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-765">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="67cb4-766">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-766">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="67cb4-767">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-767">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="67cb4-768">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-768">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-769">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-769">Profile</span></span>

* <span data-ttu-id="67cb4-770">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-770">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="67cb4-771">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67cb4-771">Service Fabric</span></span>

* <span data-ttu-id="67cb4-772">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67cb4-772">Preview release</span></span>
* <span data-ttu-id="67cb4-773">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-773">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="67cb4-774">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-774">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="67cb4-775">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-775">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-776">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-776">Storage</span></span>

* <span data-ttu-id="67cb4-777">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-777">Enabled setting blob tier</span></span>
* <span data-ttu-id="67cb4-778">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-778">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="67cb4-779">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-779">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="67cb4-780">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-780">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="67cb4-781">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-781">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="67cb4-782">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="67cb4-782">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-783">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-783">VM</span></span>

* <span data-ttu-id="67cb4-784">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-784">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="67cb4-785">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="67cb4-785">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="67cb4-786">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-786">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="67cb4-787">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="67cb4-787">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="67cb4-788">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-788">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="67cb4-789">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="67cb4-789">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="67cb4-790">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-790">August 15, 2017</span></span>

<span data-ttu-id="67cb4-791">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="67cb4-791">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-792">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-792">ACS</span></span>

* <span data-ttu-id="67cb4-793">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-793">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-794">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-794">Appservice</span></span>

* <span data-ttu-id="67cb4-795">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-795">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="67cb4-796">Event Grid</span><span class="sxs-lookup"><span data-stu-id="67cb4-796">Event Grid</span></span>

* <span data-ttu-id="67cb4-797">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-797">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="67cb4-798">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-798">August 11, 2017</span></span>

<span data-ttu-id="67cb4-799">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="67cb4-799">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-800">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-800">ACS</span></span>

* <span data-ttu-id="67cb4-801">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-801">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="67cb4-802">Batch</span><span class="sxs-lookup"><span data-stu-id="67cb4-802">Batch</span></span>

* <span data-ttu-id="67cb4-803">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-803">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="67cb4-804">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-804">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="67cb4-805">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-805">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="67cb4-806">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="67cb4-806">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="67cb4-807">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="67cb4-807">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="67cb4-808">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-808">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="67cb4-809">Komponente</span><span class="sxs-lookup"><span data-stu-id="67cb4-809">Component</span></span>

* <span data-ttu-id="67cb4-810">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-810">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="67cb4-811">Container</span><span class="sxs-lookup"><span data-stu-id="67cb4-811">Container</span></span>

* <span data-ttu-id="67cb4-812">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="67cb4-812">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="67cb4-813">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-813">Data Lake Store</span></span>

* <span data-ttu-id="67cb4-814">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-814">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="67cb4-815">Event Grid</span><span class="sxs-lookup"><span data-stu-id="67cb4-815">Event Grid</span></span>

* <span data-ttu-id="67cb4-816">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67cb4-816">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-817">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-817">Network</span></span>

* <span data-ttu-id="67cb4-818">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-818">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="67cb4-819">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="67cb4-819">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="67cb4-820">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="67cb4-820">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="67cb4-821">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="67cb4-821">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-822">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-822">Profile</span></span>

* <span data-ttu-id="67cb4-823">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="67cb4-823">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-824">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-824">Storage</span></span>

* <span data-ttu-id="67cb4-825">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-825">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-826">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-826">VM</span></span>

* <span data-ttu-id="67cb4-827">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-827">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="67cb4-828">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-828">Exposed `list-skus` command</span></span>
* <span data-ttu-id="67cb4-829">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-829">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="67cb4-830">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="67cb4-830">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="67cb4-831">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-831">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="67cb4-832">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-832">July 28, 2017</span></span>

<span data-ttu-id="67cb4-833">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="67cb4-833">Version 2.0.12</span></span>

* <span data-ttu-id="67cb4-834">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-834">Added container commands</span></span>
* <span data-ttu-id="67cb4-835">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-835">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="67cb4-836">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-836">Core</span></span>

* <span data-ttu-id="67cb4-837">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="67cb4-837">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="67cb4-838">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-838">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="67cb4-839">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="67cb4-839">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="67cb4-840">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="67cb4-840">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="67cb4-841">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="67cb4-841">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="67cb4-842">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="67cb4-842">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="67cb4-843">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="67cb4-843">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="67cb4-844">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="67cb4-844">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="67cb4-845">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="67cb4-845">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="67cb4-846">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-846">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="67cb4-847">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="67cb4-847">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="67cb4-848">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="67cb4-848">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="67cb4-849">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="67cb4-849">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="67cb4-850">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="67cb4-850">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="67cb4-851">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="67cb4-851">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="67cb4-852">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="67cb4-852">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="67cb4-853">ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-853">ACR</span></span>

* <span data-ttu-id="67cb4-854">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-854">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="67cb4-855">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-855">Support SKU update for managed registries</span></span>
* <span data-ttu-id="67cb4-856">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-856">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="67cb4-857">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-857">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="67cb4-858">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-858">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="67cb4-859">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-859">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-860">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-860">ACS</span></span>

* <span data-ttu-id="67cb4-861">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="67cb4-861">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-862">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-862">Appservice</span></span>

* <span data-ttu-id="67cb4-863">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="67cb4-863">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="67cb4-864">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="67cb4-864">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="67cb4-865">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="67cb4-865">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="67cb4-866">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="67cb4-866">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="67cb4-867">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="67cb4-867">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="67cb4-868">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="67cb4-868">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="67cb4-869">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="67cb4-869">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="67cb4-870">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="67cb4-870">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="67cb4-871">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-871">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="67cb4-872">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="67cb4-872">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="67cb4-873">Batch</span><span class="sxs-lookup"><span data-stu-id="67cb4-873">Batch</span></span>

* <span data-ttu-id="67cb4-874">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-874">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="67cb4-875">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-875">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="67cb4-876">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-876">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="67cb4-877">CDN</span><span class="sxs-lookup"><span data-stu-id="67cb4-877">CDN</span></span>

* <span data-ttu-id="67cb4-878">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="67cb4-878">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="67cb4-879">Cloud</span><span class="sxs-lookup"><span data-stu-id="67cb4-879">Cloud</span></span>

* <span data-ttu-id="67cb4-880">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="67cb4-880">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="67cb4-881">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="67cb4-881">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="67cb4-882">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="67cb4-882">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="67cb4-883">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="67cb4-883">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="67cb4-884">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67cb4-884">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67cb4-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67cb4-885">CosmosDB</span></span>

* <span data-ttu-id="67cb4-886">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="67cb4-886">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="67cb4-887">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-887">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67cb4-888">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67cb4-888">Data Lake Analytics</span></span>

* <span data-ttu-id="67cb4-889">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-889">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="67cb4-890">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-890">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="67cb4-891">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-891">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67cb4-892">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-892">Data Lake Store</span></span>

* <span data-ttu-id="67cb4-893">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-893">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="67cb4-894">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="67cb4-894">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="67cb4-895">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-895">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="67cb4-896">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="67cb4-896">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="67cb4-897">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="67cb4-897">Interactive</span></span>

* <span data-ttu-id="67cb4-898">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-898">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="67cb4-899">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-899">Increased test coverage</span></span>
* <span data-ttu-id="67cb4-900">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-900">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="67cb4-901">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="67cb4-901">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="67cb4-902">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="67cb4-902">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="67cb4-903">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="67cb4-903">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="67cb4-904">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="67cb4-904">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="67cb4-905">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-905">Added `--progress` flag</span></span>
* <span data-ttu-id="67cb4-906">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-906">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="67cb4-907">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="67cb4-907">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="67cb4-908">IoT</span><span class="sxs-lookup"><span data-stu-id="67cb4-908">IoT</span></span>

* <span data-ttu-id="67cb4-909">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="67cb4-909">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="67cb4-910">(3934)</span><span class="sxs-lookup"><span data-stu-id="67cb4-910">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="67cb4-911">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="67cb4-911">Key vault</span></span>

* <span data-ttu-id="67cb4-912">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="67cb4-912">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="67cb4-913">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67cb4-913">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="67cb4-914">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67cb4-914">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="67cb4-915">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67cb4-915">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="67cb4-916">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67cb4-916">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="67cb4-917">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="67cb4-917">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="67cb4-918">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-918">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="67cb4-919">(3307)</span><span class="sxs-lookup"><span data-stu-id="67cb4-919">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="67cb4-920">Labor</span><span class="sxs-lookup"><span data-stu-id="67cb4-920">Lab</span></span>

* <span data-ttu-id="67cb4-921">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-921">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="67cb4-922">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-922">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-923">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-923">Monitor</span></span>

* <span data-ttu-id="67cb4-924">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="67cb4-924">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="67cb4-925">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-925">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="67cb4-926">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-926">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="67cb4-927">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-927">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="67cb4-928">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67cb4-928">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="67cb4-929">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="67cb4-929">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="67cb4-930">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="67cb4-930">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="67cb4-931">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="67cb4-931">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="67cb4-932">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="67cb4-932">`location` no longer required</span></span>
  * <span data-ttu-id="67cb4-933">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="67cb4-933">Add name and ID support for target</span></span>
  * <span data-ttu-id="67cb4-934">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="67cb4-934">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="67cb4-935">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="67cb4-935">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="67cb4-936">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-936">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="67cb4-937">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="67cb4-937">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="67cb4-938">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="67cb4-938">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="67cb4-939">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-939">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-940">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-940">Network</span></span>

* <span data-ttu-id="67cb4-941">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-941">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="67cb4-942">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-942">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="67cb4-943">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67cb4-943">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="67cb4-944">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="67cb4-944">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="67cb4-945">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="67cb4-945">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="67cb4-946">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-946">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="67cb4-947">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="67cb4-947">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="67cb4-948">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="67cb4-948">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="67cb4-949">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="67cb4-949">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="67cb4-950">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="67cb4-950">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="67cb4-951">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-951">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="67cb4-952">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-952">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="67cb4-953">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="67cb4-953">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="67cb4-954">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-954">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="67cb4-955">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-955">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="67cb4-956">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-956">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="67cb4-957">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-957">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="67cb4-958">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="67cb4-958">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="67cb4-959">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-959">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="67cb4-960">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-960">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="67cb4-961">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="67cb4-961">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="67cb4-962">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67cb4-962">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="67cb4-963">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-963">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="67cb4-964">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67cb4-964">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="67cb4-965">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67cb4-965">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="67cb4-966">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67cb4-966">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="67cb4-967">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67cb4-967">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-968">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-968">Profile</span></span>

* <span data-ttu-id="67cb4-969">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="67cb4-969">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="67cb4-970">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="67cb4-970">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="67cb4-971">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="67cb4-971">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="67cb4-972">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-972">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="67cb4-973">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="67cb4-973">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="67cb4-974">RDBMS</span><span class="sxs-lookup"><span data-stu-id="67cb4-974">RDBMS</span></span>

* <span data-ttu-id="67cb4-975">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="67cb4-975">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="67cb4-976">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="67cb4-976">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="67cb4-977">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="67cb4-977">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="67cb4-978">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="67cb4-978">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-979">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-979">Resource</span></span>

* <span data-ttu-id="67cb4-980">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-980">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="67cb4-981">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="67cb4-981">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="67cb4-982">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-982">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="67cb4-983">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="67cb4-983">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="67cb4-984">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="67cb4-984">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="67cb4-985">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="67cb4-985">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="67cb4-986">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="67cb4-986">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="67cb4-987">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-987">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-988">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-988">Role</span></span>

* <span data-ttu-id="67cb4-989">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="67cb4-989">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="67cb4-990">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="67cb4-990">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="67cb4-991">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="67cb4-991">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="67cb4-992">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="67cb4-992">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="67cb4-993">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-993">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="67cb4-994">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67cb4-994">Service Fabric</span></span>
* <span data-ttu-id="67cb4-995">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="67cb4-995">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="67cb4-996">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="67cb4-996">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="67cb4-997">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="67cb4-997">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-998">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-998">SQL</span></span>

* <span data-ttu-id="67cb4-999">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-999">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="67cb4-1000">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="67cb4-1000">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="67cb4-1001">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-1001">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-1002">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-1002">Storage</span></span>

* <span data-ttu-id="67cb4-1003">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1003">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="67cb4-1004">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-1004">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="67cb4-1005">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1005">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="67cb4-1006">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1006">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="67cb4-1007">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1007">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="67cb4-1008">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1008">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-1009">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-1009">VM</span></span>

* <span data-ttu-id="67cb4-1010">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="67cb4-1010">Support configuring nsg</span></span>
* <span data-ttu-id="67cb4-1011">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="67cb4-1011">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="67cb4-1012">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="67cb4-1012">Support managed service identities</span></span>
* <span data-ttu-id="67cb4-1013">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="67cb4-1013">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="67cb4-1014">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="67cb4-1014">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="67cb4-1015">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-1015">May 10, 2017</span></span>

<span data-ttu-id="67cb4-1016">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="67cb4-1016">Version 2.0.6</span></span>

* <span data-ttu-id="67cb4-1017">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1017">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="67cb4-1018">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1018">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="67cb4-1019">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="67cb4-1019">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="67cb4-1020">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1020">Include Cognitive Services module</span></span>
* <span data-ttu-id="67cb4-1021">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1021">Include Service Fabric module</span></span>
* <span data-ttu-id="67cb4-1022">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1022">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="67cb4-1023">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="67cb4-1023">Add support for CDN commands</span></span>
* <span data-ttu-id="67cb4-1024">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1024">Remove Container module</span></span>
* <span data-ttu-id="67cb4-1025">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1025">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="67cb4-1026">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1026">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="67cb4-1027">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-1027">Core</span></span>

* <span data-ttu-id="67cb4-1028">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="67cb4-1028">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="67cb4-1029">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1029">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="67cb4-1030">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1030">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="67cb4-1031">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1031">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="67cb4-1032">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1032">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="67cb4-1033">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1033">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="67cb4-1034">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1034">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="67cb4-1035">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1035">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="67cb4-1036">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1036">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="67cb4-1037">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="67cb4-1037">core: Improved performance</span></span>
* <span data-ttu-id="67cb4-1038">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1038">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="67cb4-1039">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="67cb4-1039">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-1040">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-1040">ACS</span></span>

* <span data-ttu-id="67cb4-1041">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67cb4-1041">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="67cb4-1042">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="67cb4-1042">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="67cb4-1043">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1043">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="67cb4-1044">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1044">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-1045">AppService</span></span>

* <span data-ttu-id="67cb4-1046">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1046">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="67cb4-1047">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1047">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="67cb4-1048">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1048">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="67cb4-1049">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="67cb4-1049">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="67cb4-1050">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1050">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="67cb4-1051">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1051">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="67cb4-1052">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="67cb4-1052">support slot swap with preview</span></span>
* <span data-ttu-id="67cb4-1053">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1053">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="67cb4-1054">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1054">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67cb4-1055">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67cb4-1055">CosmosDB</span></span>

* <span data-ttu-id="67cb4-1056">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="67cb4-1056">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="67cb4-1057">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="67cb4-1057">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="67cb4-1058">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="67cb4-1058">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="67cb4-1059">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="67cb4-1059">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67cb4-1060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67cb4-1060">Data Lake Analytics</span></span>

* <span data-ttu-id="67cb4-1061">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="67cb4-1061">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="67cb4-1062">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1062">Add support for new catalog item type: package.</span></span> <span data-ttu-id="67cb4-1063">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1063">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="67cb4-1064">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="67cb4-1064">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="67cb4-1065">Table</span><span class="sxs-lookup"><span data-stu-id="67cb4-1065">Table</span></span>
  * <span data-ttu-id="67cb4-1066">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="67cb4-1066">Table valued function</span></span>
  * <span data-ttu-id="67cb4-1067">Sicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-1067">View</span></span>
  * <span data-ttu-id="67cb4-1068">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1068">Table Statistics.</span></span> <span data-ttu-id="67cb4-1069">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1069">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67cb4-1070">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-1070">Data Lake Store</span></span>

* <span data-ttu-id="67cb4-1071">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-1071">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="67cb4-1072">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1072">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="67cb4-1073">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="67cb4-1073">missed help for access show.</span></span> <span data-ttu-id="67cb4-1074">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67cb4-1074">adding it.</span></span> <span data-ttu-id="67cb4-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="67cb4-1076">Suchen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1076">Find</span></span>

* <span data-ttu-id="67cb4-1077">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="67cb4-1077">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="67cb4-1078">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67cb4-1078">KeyVault</span></span>

* <span data-ttu-id="67cb4-1079">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1079">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="67cb4-1080">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="67cb4-1080">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="67cb4-1081">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="67cb4-1081">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="67cb4-1082">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="67cb4-1082">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="67cb4-1083">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1083">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="67cb4-1084">Labor</span><span class="sxs-lookup"><span data-stu-id="67cb4-1084">Lab</span></span>

* <span data-ttu-id="67cb4-1085">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="67cb4-1085">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="67cb4-1086">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="67cb4-1086">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="67cb4-1087">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="67cb4-1087">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="67cb4-1088">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="67cb4-1088">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="67cb4-1089">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="67cb4-1089">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="67cb4-1090">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1090">Monitor</span></span>

* <span data-ttu-id="67cb4-1091">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1091">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="67cb4-1092">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1092">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="67cb4-1093">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-1093">Network</span></span>

* <span data-ttu-id="67cb4-1094">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1094">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="67cb4-1095">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1095">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="67cb4-1096">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="67cb4-1096">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="67cb4-1097">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1097">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="67cb4-1098">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="67cb4-1098">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="67cb4-1099">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="67cb4-1099">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="67cb4-1100">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1100">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="67cb4-1101">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1101">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="67cb4-1102">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1102">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="67cb4-1103">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="67cb4-1103">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="67cb4-1104">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1104">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="67cb4-1105">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1105">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="67cb4-1106">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="67cb4-1106">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="67cb4-1107">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="67cb4-1107">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="67cb4-1108">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="67cb4-1108">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="67cb4-1109">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1109">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="67cb4-1110">Profil</span><span class="sxs-lookup"><span data-stu-id="67cb4-1110">Profile</span></span>

* <span data-ttu-id="67cb4-1111">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1111">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="67cb4-1112">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1112">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="67cb4-1113">Redis</span><span class="sxs-lookup"><span data-stu-id="67cb4-1113">Redis</span></span>

* <span data-ttu-id="67cb4-1114">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-1114">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="67cb4-1115">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1115">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="67cb4-1116">Ressource</span><span class="sxs-lookup"><span data-stu-id="67cb4-1116">Resource</span></span>

* <span data-ttu-id="67cb4-1117">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1117">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="67cb4-1118">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1118">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="67cb4-1119">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1119">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="67cb4-1120">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="67cb4-1120">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="67cb4-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="67cb4-1122">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1122">Add docs for az lock update.</span></span> <span data-ttu-id="67cb4-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="67cb4-1124">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="67cb4-1124">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="67cb4-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="67cb4-1126">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="67cb4-1126">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="67cb4-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="67cb4-1128">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1128">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="67cb4-1129">Rolle</span><span class="sxs-lookup"><span data-stu-id="67cb4-1129">Role</span></span>

* <span data-ttu-id="67cb4-1130">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1130">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="67cb4-1131">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1131">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="67cb4-1132">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1132">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="67cb4-1133">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="67cb4-1133">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="67cb4-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="67cb4-1134">SQL</span></span>

* <span data-ttu-id="67cb4-1135">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1135">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="67cb4-1136">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1136">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="67cb4-1137">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-1137">Storage</span></span>

* <span data-ttu-id="67cb4-1138">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1138">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="67cb4-1139">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="67cb4-1139">Add support for incremental blob copy</span></span>
* <span data-ttu-id="67cb4-1140">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="67cb4-1140">Add support for large block blob upload</span></span>
* <span data-ttu-id="67cb4-1141">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="67cb4-1141">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-1142">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-1142">VM</span></span>

* <span data-ttu-id="67cb4-1143">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="67cb4-1143">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="67cb4-1144">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="67cb4-1144">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="67cb4-1145">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="67cb4-1145">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="67cb4-1146">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="67cb4-1146">az vm/vmss disk</span></span>
  3. <span data-ttu-id="67cb4-1147">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1147">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="67cb4-1148">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="67cb4-1148">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="67cb4-1149">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1149">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="67cb4-1150">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-1150">April 3, 2017</span></span>

<span data-ttu-id="67cb4-1151">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="67cb4-1151">Version 2.0.2</span></span>

<span data-ttu-id="67cb4-1152">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1152">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="67cb4-1153">Core</span><span class="sxs-lookup"><span data-stu-id="67cb4-1153">Core</span></span>

* <span data-ttu-id="67cb4-1154">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="67cb4-1154">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="67cb4-1155">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1155">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="67cb4-1156">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1156">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="67cb4-1157">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1157">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="67cb4-1158">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1158">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="67cb4-1159">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="67cb4-1159">Add prompting for missing template parameters.</span></span> <span data-ttu-id="67cb4-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="67cb4-1161">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-1161">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="67cb4-1162">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="67cb4-1162">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="67cb4-1163">ACS</span><span class="sxs-lookup"><span data-stu-id="67cb4-1163">ACS</span></span>

* <span data-ttu-id="67cb4-1164">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1164">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="67cb4-1165">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="67cb4-1165">Add support for ssh key password prompting.</span></span> <span data-ttu-id="67cb4-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="67cb4-1167">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="67cb4-1167">Add support for windows clusters.</span></span> <span data-ttu-id="67cb4-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="67cb4-1169">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="67cb4-1169">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="67cb4-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="67cb4-1171">AppService</span><span class="sxs-lookup"><span data-stu-id="67cb4-1171">AppService</span></span>

* <span data-ttu-id="67cb4-1172">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1172">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="67cb4-1173">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1173">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="67cb4-1174">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1174">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="67cb4-1175">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1175">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="67cb4-1176">DataLake</span><span class="sxs-lookup"><span data-stu-id="67cb4-1176">DataLake</span></span>

* <span data-ttu-id="67cb4-1177">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1177">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="67cb4-1178">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="67cb4-1178">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="67cb4-1179">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="67cb4-1179">DocuemntDB</span></span>

* <span data-ttu-id="67cb4-1180">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1180">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="67cb4-1181">VM</span><span class="sxs-lookup"><span data-stu-id="67cb4-1181">VM</span></span>

* <span data-ttu-id="67cb4-1182">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1182">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="67cb4-1183">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1183">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="67cb4-1184">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1184">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="67cb4-1185">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1185">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="67cb4-1186">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1186">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="67cb4-1187">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1187">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="67cb4-1188">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="67cb4-1188">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="67cb4-1189">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="67cb4-1189">February 27, 2017</span></span>

<span data-ttu-id="67cb4-1190">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="67cb4-1190">Version 2.0.0</span></span>

<span data-ttu-id="67cb4-1191">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="67cb4-1191">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="67cb4-1192">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1192">Container Service (acs)</span></span>
- <span data-ttu-id="67cb4-1193">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1193">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="67cb4-1194">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67cb4-1194">Networking</span></span>
- <span data-ttu-id="67cb4-1195">Speicher</span><span class="sxs-lookup"><span data-stu-id="67cb4-1195">Storage</span></span>

<span data-ttu-id="67cb4-1196">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1196">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="67cb4-1197">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1197">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="67cb4-1198">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1198">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="67cb4-1199">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="67cb4-1199">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="67cb4-1200">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="67cb4-1200">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="67cb4-1201">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="67cb4-1201">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="67cb4-1202">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1202">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="67cb4-1203">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="67cb4-1203">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="67cb4-1204">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="67cb4-1204">Provide feedback from the command line with the `az feedback` command</span></span>

