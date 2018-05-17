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
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="e00d8-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="e00d8-103">Azure CLI 2.0 release notes</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e00d8-104">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-104">May 7, 2018</span></span>

<span data-ttu-id="e00d8-105">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e00d8-105">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-106">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-106">Core</span></span>

* <span data-ttu-id="e00d8-107">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="e00d8-107">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e00d8-108">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-108">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e00d8-109">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e00d8-109">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e00d8-110">#5591</span><span class="sxs-lookup"><span data-stu-id="e00d8-110">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e00d8-111">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-111">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e00d8-112">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="e00d8-112">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e00d8-113">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="e00d8-113">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e00d8-114">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="e00d8-114">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e00d8-115">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-115">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-116">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-116">ACR</span></span>

* <span data-ttu-id="e00d8-117">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-117">Added ACR Build commands</span></span>
* <span data-ttu-id="e00d8-118">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-118">Improved resource not found error messages</span></span>
* <span data-ttu-id="e00d8-119">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="e00d8-119">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e00d8-120">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-120">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e00d8-121">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-121">Improved repository commands error messages</span></span>
* <span data-ttu-id="e00d8-122">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-122">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-123">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-123">ACS</span></span>

* <span data-ttu-id="e00d8-124">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-124">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e00d8-125">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-125">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e00d8-126">AMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-126">AMS</span></span>

* <span data-ttu-id="e00d8-127">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="e00d8-127">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-128">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-128">Appservice</span></span>

* <span data-ttu-id="e00d8-129">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="e00d8-129">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e00d8-130">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-130">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e00d8-131">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-131">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e00d8-132">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-132">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e00d8-133">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e00d8-133">Batch AI</span></span>

* <span data-ttu-id="e00d8-134">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-134">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e00d8-135">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e00d8-135">Cognitive Services</span></span>

* <span data-ttu-id="e00d8-136">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="e00d8-136">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e00d8-137">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e00d8-137">Consumption</span></span>

* <span data-ttu-id="e00d8-138">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-138">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-139">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-139">Container</span></span>

* <span data-ttu-id="e00d8-140">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e00d8-140">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e00d8-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e00d8-141">Cosmos DB</span></span>

* <span data-ttu-id="e00d8-142">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e00d8-142">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e00d8-143">DMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-143">DMS</span></span>

* <span data-ttu-id="e00d8-144">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-144">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-145">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-145">Extension</span></span>

* <span data-ttu-id="e00d8-146">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-146">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-147">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-147">Interactive</span></span>

* <span data-ttu-id="e00d8-148">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="e00d8-148">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e00d8-149">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="e00d8-149">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e00d8-150">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-150">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e00d8-151">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-151">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e00d8-152">Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-152">Lab</span></span>

* <span data-ttu-id="e00d8-153">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-153">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-154">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-154">Network</span></span>

* <span data-ttu-id="e00d8-155">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="e00d8-155">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e00d8-156">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-156">Profile</span></span>

* <span data-ttu-id="e00d8-157">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-157">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e00d8-158">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-158">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e00d8-159">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-159">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e00d8-160">Redis</span><span class="sxs-lookup"><span data-stu-id="e00d8-160">Redis</span></span>

* <span data-ttu-id="e00d8-161">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-161">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e00d8-162">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-162">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e00d8-163">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="e00d8-163">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e00d8-164">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-164">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e00d8-165">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-165">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-166">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-166">Role</span></span>

* <span data-ttu-id="e00d8-167">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-167">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-168">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-168">Storage</span></span>

* <span data-ttu-id="e00d8-169">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-169">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e00d8-170">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="e00d8-170">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e00d8-171">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="e00d8-171">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e00d8-172">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="e00d8-172">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e00d8-173">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e00d8-173">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-174">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-174">VM</span></span>

* <span data-ttu-id="e00d8-175">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-175">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e00d8-176">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-176">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e00d8-177">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="e00d8-177">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e00d8-178">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-178">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e00d8-179">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="e00d8-179">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e00d8-180">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-180">Added write accelerator support</span></span> 
* <span data-ttu-id="e00d8-181">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-181">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e00d8-182">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="e00d8-182">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e00d8-183">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="e00d8-183">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e00d8-184">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-184">April 10, 2018</span></span>

<span data-ttu-id="e00d8-185">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e00d8-185">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-186">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-186">ACR</span></span>

* <span data-ttu-id="e00d8-187">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="e00d8-187">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-188">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-188">ACS</span></span>

* <span data-ttu-id="e00d8-189">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-189">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-190">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-190">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e00d8-192">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-192">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e00d8-193">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e00d8-193">BatchAI</span></span>

* <span data-ttu-id="e00d8-194">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-194">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="e00d8-195">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="e00d8-195">Job level mounting</span></span>
 - <span data-ttu-id="e00d8-196">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="e00d8-196">Environment variables with secret values</span></span>
 - <span data-ttu-id="e00d8-197">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="e00d8-197">Performance counters settings</span></span>
 - <span data-ttu-id="e00d8-198">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="e00d8-198">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="e00d8-199">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="e00d8-199">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="e00d8-200">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="e00d8-200">Usage and limits reporting</span></span>
 - <span data-ttu-id="e00d8-201">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="e00d8-201">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="e00d8-202">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="e00d8-202">Support for custom images</span></span>
 - <span data-ttu-id="e00d8-203">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-203">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e00d8-204">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="e00d8-204">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e00d8-205">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-205">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e00d8-206">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="e00d8-206">National clouds are supported</span></span>
* <span data-ttu-id="e00d8-207">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-207">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e00d8-208">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="e00d8-208">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e00d8-209">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-209">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e00d8-210">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="e00d8-210">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e00d8-211">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="e00d8-211">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e00d8-212">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="e00d8-212">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e00d8-213">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="e00d8-213">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e00d8-214">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-214">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e00d8-215">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="e00d8-215">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e00d8-216">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-216">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e00d8-217">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="e00d8-217">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e00d8-218">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-218">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e00d8-219">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="e00d8-219">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e00d8-220">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e00d8-220">Billing</span></span>

* <span data-ttu-id="e00d8-221">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-221">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e00d8-222">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e00d8-222">Consumption</span></span>

* <span data-ttu-id="e00d8-223">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-223">Added `marketplace` commands</span></span>
* <span data-ttu-id="e00d8-224">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-224">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e00d8-225">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-225">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e00d8-226">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-226">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e00d8-227">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-227">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e00d8-228">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-228">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-229">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-229">Container</span></span>

* <span data-ttu-id="e00d8-230">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-230">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e00d8-231">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e00d8-231">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-232">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-232">Extension</span></span>

* <span data-ttu-id="e00d8-233">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-233">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-234">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-234">Interactive</span></span>

* <span data-ttu-id="e00d8-235">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="e00d8-235">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e00d8-236">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-236">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e00d8-237">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-237">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-238">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-238">Network</span></span>

* <span data-ttu-id="e00d8-239">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-239">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e00d8-240">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-240">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e00d8-241">#4910</span><span class="sxs-lookup"><span data-stu-id="e00d8-241">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e00d8-242">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-242">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="e00d8-243">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-243">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e00d8-244">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-244">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e00d8-245">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-245">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e00d8-246">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-246">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-247">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-247">Profile</span></span>

* <span data-ttu-id="e00d8-248">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-248">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e00d8-249">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-249">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00d8-250">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-250">RDBMS</span></span>

* <span data-ttu-id="e00d8-251">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-251">Added `georestore` command</span></span>
* <span data-ttu-id="e00d8-252">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-252">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-253">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-253">Resource</span></span>

* <span data-ttu-id="e00d8-254">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-254">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e00d8-255">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-255">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-256">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-256">SQL</span></span>

* <span data-ttu-id="e00d8-257">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-257">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-258">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-258">Storage</span></span>

* <span data-ttu-id="e00d8-259">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-259">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-260">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-260">VM</span></span>

* <span data-ttu-id="e00d8-261">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-261">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e00d8-262">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-262">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e00d8-264">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-264">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e00d8-265">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="e00d8-265">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e00d8-266">#5718</span><span class="sxs-lookup"><span data-stu-id="e00d8-266">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e00d8-267">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="e00d8-267">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e00d8-268">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-268">March 27, 2018</span></span>

<span data-ttu-id="e00d8-269">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e00d8-269">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-270">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-270">Core</span></span>

* <span data-ttu-id="e00d8-271">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="e00d8-271">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-272">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-272">ACS</span></span>

* <span data-ttu-id="e00d8-273">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e00d8-273">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-274">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-274">Appservice</span></span>

* <span data-ttu-id="e00d8-275">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-275">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e00d8-276">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-276">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e00d8-277">Backup</span><span class="sxs-lookup"><span data-stu-id="e00d8-277">Backup</span></span>

* <span data-ttu-id="e00d8-278">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-278">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e00d8-279">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="e00d8-279">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e00d8-280">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="e00d8-280">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e00d8-281">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="e00d8-281">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-282">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-282">Container</span></span>

* <span data-ttu-id="e00d8-283">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-283">Added `container exec` command.</span></span> <span data-ttu-id="e00d8-284">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e00d8-284">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e00d8-285">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e00d8-285">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-286">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-286">Extension</span></span>

* <span data-ttu-id="e00d8-287">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="e00d8-287">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e00d8-288">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e00d8-288">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e00d8-289">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e00d8-289">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-290">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-290">Interactive</span></span>

* <span data-ttu-id="e00d8-291">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="e00d8-291">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e00d8-292">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-292">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e00d8-293">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e00d8-293">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e00d8-294">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="e00d8-294">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e00d8-295">Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-295">Lab</span></span>

* <span data-ttu-id="e00d8-296">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-296">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-297">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-297">Monitor</span></span>

* <span data-ttu-id="e00d8-298">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="e00d8-298">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e00d8-299">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="e00d8-299">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e00d8-300">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="e00d8-300">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-301">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-301">Network</span></span>

* <span data-ttu-id="e00d8-302">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-302">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-303">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-303">Profile</span></span>

* <span data-ttu-id="e00d8-304">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-304">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00d8-305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-305">RDBMS</span></span>

* <span data-ttu-id="e00d8-306">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-306">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-307">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-307">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e00d8-309">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-309">Role</span></span>

* <span data-ttu-id="e00d8-310">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-310">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e00d8-311">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e00d8-311">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e00d8-312">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-312">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e00d8-313">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-313">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e00d8-314">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-314">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-315">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-315">Storage</span></span>

* <span data-ttu-id="e00d8-316">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-316">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e00d8-317">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="e00d8-317">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-318">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-318">VM</span></span>

* <span data-ttu-id="e00d8-319">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-319">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e00d8-320">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-320">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e00d8-321">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="e00d8-321">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e00d8-322">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e00d8-322">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e00d8-323">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-323">March 13, 2018</span></span>

<span data-ttu-id="e00d8-324">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e00d8-324">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-325">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-325">ACR</span></span>

* <span data-ttu-id="e00d8-326">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-326">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e00d8-327">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-327">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e00d8-328">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-328">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-329">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-329">ACS</span></span>

* <span data-ttu-id="e00d8-330">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-330">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e00d8-331">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-331">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e00d8-332">Advisor</span><span class="sxs-lookup"><span data-stu-id="e00d8-332">Advisor</span></span>

* <span data-ttu-id="e00d8-333">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-333">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e00d8-334">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-334">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e00d8-335">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-335">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="e00d8-336">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-336">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e00d8-337">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-337">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-338">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-338">Appservice</span></span>

* <span data-ttu-id="e00d8-339">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-339">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e00d8-340">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-340">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e00d8-341">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="e00d8-341">Eventhubs</span></span>

* <span data-ttu-id="e00d8-342">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-342">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-343">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-343">Extension</span></span>

* <span data-ttu-id="e00d8-344">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="e00d8-344">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-345">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-345">Interactive</span></span>

* <span data-ttu-id="e00d8-346">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="e00d8-346">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e00d8-347">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="e00d8-347">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e00d8-348">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="e00d8-348">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e00d8-349">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-349">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-350">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-350">Monitor</span></span>

* <span data-ttu-id="e00d8-351">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-351">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e00d8-352">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-352">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e00d8-353">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-353">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e00d8-354">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-354">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-355">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-355">Network</span></span>

* <span data-ttu-id="e00d8-356">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-356">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e00d8-357">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="e00d8-357">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e00d8-358">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-358">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e00d8-359">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-359">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-360">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-360">Profile</span></span>

* <span data-ttu-id="e00d8-361">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-361">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e00d8-362">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-362">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00d8-363">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-363">RDBMS</span></span>

* <span data-ttu-id="e00d8-364">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-364">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e00d8-365">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e00d8-365">Service Bus</span></span>

* <span data-ttu-id="e00d8-366">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-366">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-367">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-367">Storage</span></span>

* <span data-ttu-id="e00d8-368">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="e00d8-368">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e00d8-369">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="e00d8-369">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-370">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-370">VM</span></span>

* <span data-ttu-id="e00d8-371">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="e00d8-371">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e00d8-372">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-372">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e00d8-373">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-373">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e00d8-374">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-374">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e00d8-375">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-375">February 27, 2018</span></span>

<span data-ttu-id="e00d8-376">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e00d8-376">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-377">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-377">Core</span></span>

* <span data-ttu-id="e00d8-378">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-378">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e00d8-379">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-379">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e00d8-380">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-380">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-381">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-381">ACS</span></span>

* <span data-ttu-id="e00d8-382">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-382">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e00d8-383">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e00d8-383">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e00d8-384">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-384">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e00d8-385">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-385">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-386">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-386">Appservice</span></span>

* <span data-ttu-id="e00d8-387">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e00d8-387">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e00d8-388">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="e00d8-388">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e00d8-389">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e00d8-389">Cognitive Services</span></span>

* <span data-ttu-id="e00d8-390">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-390">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e00d8-391">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e00d8-391">Consumption</span></span>

* <span data-ttu-id="e00d8-392">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-392">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e00d8-393">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-393">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-394">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-394">Container</span></span>

* <span data-ttu-id="e00d8-395">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="e00d8-395">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-396">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-396">Network</span></span>

* <span data-ttu-id="e00d8-397">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e00d8-397">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-398">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-398">Resource</span></span>

* <span data-ttu-id="e00d8-399">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="e00d8-399">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-400">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-400">Role</span></span>

* <span data-ttu-id="e00d8-401">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-401">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-402">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-402">SQL</span></span>

* <span data-ttu-id="e00d8-403">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="e00d8-403">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-404">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-404">Storage</span></span>

* <span data-ttu-id="e00d8-405">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-405">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-406">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-406">VM</span></span>

* <span data-ttu-id="e00d8-407">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-407">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e00d8-408">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-408">February 13, 2018</span></span>

<span data-ttu-id="e00d8-409">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e00d8-409">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-410">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-410">Core</span></span>

* <span data-ttu-id="e00d8-411">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-411">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-412">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-412">ACS</span></span>

* <span data-ttu-id="e00d8-413">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-413">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e00d8-414">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-414">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e00d8-415">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-415">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e00d8-416">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-416">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e00d8-417">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-417">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e00d8-418">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-418">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e00d8-419">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="e00d8-419">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e00d8-420">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="e00d8-420">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-421">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-421">Appservice</span></span>

* <span data-ttu-id="e00d8-422">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="e00d8-422">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e00d8-423">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-423">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e00d8-424">CDN</span><span class="sxs-lookup"><span data-stu-id="e00d8-424">CDN</span></span>

* <span data-ttu-id="e00d8-425">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-425">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-426">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-426">Container</span></span>

* <span data-ttu-id="e00d8-427">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-427">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e00d8-428">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-428">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00d8-429">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00d8-429">CosmosDB</span></span>

* <span data-ttu-id="e00d8-430">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-430">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-431">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-431">Extension</span></span>

* <span data-ttu-id="e00d8-432">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-432">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e00d8-433">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-433">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e00d8-434">Feedback</span><span class="sxs-lookup"><span data-stu-id="e00d8-434">Feedback</span></span>

* <span data-ttu-id="e00d8-435">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-435">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-436">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-436">Interactive</span></span>

* <span data-ttu-id="e00d8-437">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-437">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e00d8-438">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-438">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e00d8-439">IoT</span><span class="sxs-lookup"><span data-stu-id="e00d8-439">IoT</span></span>

* <span data-ttu-id="e00d8-440">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="e00d8-440">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e00d8-441">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="e00d8-441">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e00d8-442">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-442">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e00d8-443">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-443">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-444">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-444">Monitor</span></span>

* <span data-ttu-id="e00d8-445">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-445">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-446">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-446">Network</span></span>

* <span data-ttu-id="e00d8-447">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="e00d8-447">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e00d8-448">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-448">Profile</span></span>

* <span data-ttu-id="e00d8-449">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="e00d8-449">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-450">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-450">Resource</span></span>

* <span data-ttu-id="e00d8-451">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-451">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-452">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-452">Role</span></span>

* <span data-ttu-id="e00d8-453">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-453">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-454">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-454">SQL</span></span>

* <span data-ttu-id="e00d8-455">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-455">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e00d8-456">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-456">Added `sql db rename`</span></span>
* <span data-ttu-id="e00d8-457">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-457">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-458">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-458">Storage</span></span>

* <span data-ttu-id="e00d8-459">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-459">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-460">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-460">VM</span></span>

* <span data-ttu-id="e00d8-461">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-461">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e00d8-462">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-462">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e00d8-463">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e00d8-463">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e00d8-464">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-464">January 31, 2018</span></span>

<span data-ttu-id="e00d8-465">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e00d8-465">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-466">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-466">Core</span></span>

* <span data-ttu-id="e00d8-467">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-467">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e00d8-468">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-468">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e00d8-469">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="e00d8-469">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e00d8-470">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="e00d8-470">Use `--verbose` to see</span></span>
* <span data-ttu-id="e00d8-471">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-471">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-472">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-472">ACS</span></span>

* <span data-ttu-id="e00d8-473">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="e00d8-473">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e00d8-474">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-474">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-475">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-475">Appservice</span></span>

* <span data-ttu-id="e00d8-476">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e00d8-476">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e00d8-477">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-477">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e00d8-478">CDN</span><span class="sxs-lookup"><span data-stu-id="e00d8-478">CDN</span></span>

* <span data-ttu-id="e00d8-479">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-479">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00d8-480">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00d8-480">CosmosDB</span></span>

* <span data-ttu-id="e00d8-481">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-481">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-482">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-482">Interactive</span></span>

* <span data-ttu-id="e00d8-483">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-483">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-484">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-484">Network</span></span>

* <span data-ttu-id="e00d8-485">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-485">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e00d8-486">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="e00d8-486">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e00d8-487">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-487">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e00d8-488">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-488">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e00d8-489">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-489">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e00d8-490">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="e00d8-490">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e00d8-491">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-491">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e00d8-492">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-492">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e00d8-493">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-493">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="e00d8-494">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="e00d8-494">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-495">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-495">Profile</span></span>

* <span data-ttu-id="e00d8-496">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-496">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-497">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-497">Resource</span></span>

* <span data-ttu-id="e00d8-498">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="e00d8-498">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-499">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-499">Storage</span></span>

* <span data-ttu-id="e00d8-500">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-500">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e00d8-501">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-501">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e00d8-502">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e00d8-502">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="e00d8-503">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-503">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e00d8-504">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="e00d8-504">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-505">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-505">VM</span></span>

* <span data-ttu-id="e00d8-506">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-506">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e00d8-507">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="e00d8-507">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e00d8-508">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-508">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e00d8-509">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-509">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e00d8-510">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="e00d8-510">January 17, 2018</span></span>

<span data-ttu-id="e00d8-511">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e00d8-511">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-512">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-512">ACR</span></span>

* <span data-ttu-id="e00d8-513">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-513">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e00d8-514">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="e00d8-514">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-515">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-515">ACS</span></span>

* <span data-ttu-id="e00d8-516">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-516">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e00d8-517">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-517">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-518">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-518">Appservice</span></span>

* <span data-ttu-id="e00d8-519">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="e00d8-519">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e00d8-520">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-520">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e00d8-521">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-521">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e00d8-522">Backup</span><span class="sxs-lookup"><span data-stu-id="e00d8-522">Backup</span></span>

* <span data-ttu-id="e00d8-523">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="e00d8-523">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e00d8-524">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-524">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e00d8-525">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="e00d8-525">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e00d8-526">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="e00d8-526">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e00d8-527">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="e00d8-527">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e00d8-528">Batch</span><span class="sxs-lookup"><span data-stu-id="e00d8-528">Batch</span></span>

* <span data-ttu-id="e00d8-529">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e00d8-529">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e00d8-530">Cloud</span><span class="sxs-lookup"><span data-stu-id="e00d8-530">Cloud</span></span>

* <span data-ttu-id="e00d8-531">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-531">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e00d8-532">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e00d8-532">Consumption</span></span>

* <span data-ttu-id="e00d8-533">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e00d8-533">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00d8-534">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e00d8-534">Event Grid</span></span>

* <span data-ttu-id="e00d8-535">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="e00d8-535">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e00d8-536">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="e00d8-536">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e00d8-537">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-537">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e00d8-538">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="e00d8-538">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e00d8-539">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-539">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e00d8-540">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-540">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e00d8-541">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-541">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e00d8-542">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-542">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-543">Interactive</span><span class="sxs-lookup"><span data-stu-id="e00d8-543">Interactive</span></span>

* <span data-ttu-id="e00d8-544">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e00d8-544">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e00d8-545">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-545">Fixed errors on startup</span></span>
* <span data-ttu-id="e00d8-546">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="e00d8-546">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e00d8-547">IoT</span><span class="sxs-lookup"><span data-stu-id="e00d8-547">IoT</span></span>

* <span data-ttu-id="e00d8-548">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-548">Added support for device provisioning service</span></span>
* <span data-ttu-id="e00d8-549">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-549">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e00d8-550">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="e00d8-550">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-551">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-551">Monitor</span></span>

* <span data-ttu-id="e00d8-552">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-552">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e00d8-553">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e00d8-553">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e00d8-554">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-554">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-555">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-555">Network</span></span>

* <span data-ttu-id="e00d8-556">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="e00d8-556">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e00d8-557">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-557">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-558">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-558">Profile</span></span>

* <span data-ttu-id="e00d8-559">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-559">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-560">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-560">Role</span></span>

* <span data-ttu-id="e00d8-561">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="e00d8-561">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00d8-562">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00d8-562">Service Fabric</span></span>

* <span data-ttu-id="e00d8-563">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-563">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e00d8-564">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-564">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-565">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-565">VM</span></span>

* <span data-ttu-id="e00d8-566">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="e00d8-566">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e00d8-567">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-567">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e00d8-568">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="e00d8-568">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e00d8-569">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-569">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e00d8-570">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-570">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e00d8-571">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-571">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00d8-572">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-572">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00d8-573">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-573">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e00d8-574">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-574">December 19, 2017</span></span>

<span data-ttu-id="e00d8-575">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e00d8-575">Version 2.0.23</span></span>

* <span data-ttu-id="e00d8-576">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-576">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-577">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-577">Container</span></span>

* <span data-ttu-id="e00d8-578">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-578">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-579">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-579">Network</span></span>

* <span data-ttu-id="e00d8-580">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-580">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e00d8-581">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-581">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-582">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-582">Storage</span></span>

* <span data-ttu-id="e00d8-583">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-583">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-584">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-584">VM</span></span>

* <span data-ttu-id="e00d8-585">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-585">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e00d8-586">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-586">December 5, 2017</span></span>

<span data-ttu-id="e00d8-587">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e00d8-587">Version 2.0.22</span></span>

* <span data-ttu-id="e00d8-588">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-588">Removed `az component` commands.</span></span> <span data-ttu-id="e00d8-589">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="e00d8-589">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-590">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-590">Core</span></span>
* <span data-ttu-id="e00d8-591">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="e00d8-591">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e00d8-592">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-592">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-593">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-593">ACS</span></span>

* <span data-ttu-id="e00d8-594">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-594">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e00d8-595">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="e00d8-595">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e00d8-596">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="e00d8-596">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e00d8-597">Advisor</span><span class="sxs-lookup"><span data-stu-id="e00d8-597">Advisor</span></span>

* <span data-ttu-id="e00d8-598">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-598">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-599">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-599">Appservice</span></span>

* <span data-ttu-id="e00d8-600">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e00d8-600">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e00d8-601">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e00d8-601">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e00d8-602">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-602">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e00d8-603">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e00d8-603">Consumption</span></span>

* <span data-ttu-id="e00d8-604">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-604">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-605">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-605">Container</span></span>

* <span data-ttu-id="e00d8-606">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="e00d8-606">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-607">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-607">Monitor</span></span>

* <span data-ttu-id="e00d8-608">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-608">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-609">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-609">Resource</span></span>

* <span data-ttu-id="e00d8-610">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-610">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-611">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-611">Role</span></span>

* <span data-ttu-id="e00d8-612">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-612">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e00d8-613">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-613">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e00d8-614">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e00d8-614">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-615">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-615">SQL</span></span>

* <span data-ttu-id="e00d8-616">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-616">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e00d8-617">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-617">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-618">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-618">VM</span></span>

* <span data-ttu-id="e00d8-619">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-619">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e00d8-620">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-620">November 14, 2017</span></span>

<span data-ttu-id="e00d8-621">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e00d8-621">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-622">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-622">ACR</span></span>

* <span data-ttu-id="e00d8-623">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-623">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e00d8-624">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-624">ACS</span></span>

* <span data-ttu-id="e00d8-625">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-625">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e00d8-626">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="e00d8-626">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e00d8-627">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="e00d8-627">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e00d8-628">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-628">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e00d8-629">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-629">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-630">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-630">Appservice</span></span>

* <span data-ttu-id="e00d8-631">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-631">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e00d8-632">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-632">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e00d8-633">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-633">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e00d8-634">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-634">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e00d8-635">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-635">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e00d8-636">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e00d8-636">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e00d8-637">Batch</span><span class="sxs-lookup"><span data-stu-id="e00d8-637">Batch</span></span>

* <span data-ttu-id="e00d8-638">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-638">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e00d8-639">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e00d8-639">Batchai</span></span>

* <span data-ttu-id="e00d8-640">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-640">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e00d8-641">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-641">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e00d8-642">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-642">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e00d8-643">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-643">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e00d8-644">Cloud</span><span class="sxs-lookup"><span data-stu-id="e00d8-644">Cloud</span></span>

* <span data-ttu-id="e00d8-645">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="e00d8-645">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-646">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-646">Container</span></span>

* <span data-ttu-id="e00d8-647">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-647">Added support to open multiple ports</span></span>
* <span data-ttu-id="e00d8-648">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-648">Added container group restart policy</span></span>
* <span data-ttu-id="e00d8-649">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-649">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e00d8-650">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-650">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00d8-651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00d8-651">Data Lake Analytics</span></span>

* <span data-ttu-id="e00d8-652">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="e00d8-652">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00d8-653">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00d8-653">Data Lake Store</span></span>

* <span data-ttu-id="e00d8-654">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="e00d8-654">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-655">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-655">Extension</span></span>

* <span data-ttu-id="e00d8-656">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-656">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e00d8-657">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e00d8-657">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e00d8-658">IoT</span><span class="sxs-lookup"><span data-stu-id="e00d8-658">IoT</span></span>

* <span data-ttu-id="e00d8-659">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-659">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-660">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-660">Monitor</span></span>

* <span data-ttu-id="e00d8-661">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-661">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-662">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-662">Network</span></span>

* <span data-ttu-id="e00d8-663">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-663">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e00d8-664">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="e00d8-664">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e00d8-665">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e00d8-665">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e00d8-666">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-666">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e00d8-667">Reservations</span><span class="sxs-lookup"><span data-stu-id="e00d8-667">Reservations</span></span>

* <span data-ttu-id="e00d8-668">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e00d8-668">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-669">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-669">Resource</span></span>

* <span data-ttu-id="e00d8-670">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-670">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-671">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-671">SQL</span></span>

* <span data-ttu-id="e00d8-672">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-672">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-673">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-673">Storage</span></span>

* <span data-ttu-id="e00d8-674">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-674">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e00d8-675">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="e00d8-675">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e00d8-676">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e00d8-676">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e00d8-677">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-677">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e00d8-678">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-678">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e00d8-679">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-679">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e00d8-680">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-680">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-681">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-681">VM</span></span>

* <span data-ttu-id="e00d8-682">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e00d8-682">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e00d8-683">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-683">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e00d8-684">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="e00d8-684">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e00d8-685">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-685">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e00d8-686">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-686">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e00d8-687">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-687">October 24, 2017</span></span>

<span data-ttu-id="e00d8-688">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e00d8-688">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-689">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-689">Core</span></span>

* <span data-ttu-id="e00d8-690">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="e00d8-690">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-691">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-691">ACR</span></span>

* <span data-ttu-id="e00d8-692">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="e00d8-692">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e00d8-693">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="e00d8-693">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e00d8-694">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-694">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-695">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-695">ACS</span></span>

* <span data-ttu-id="e00d8-696">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-696">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e00d8-697">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-697">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-698">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-698">Appservice</span></span>

* <span data-ttu-id="e00d8-699">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="e00d8-699">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e00d8-700">Komponente</span><span class="sxs-lookup"><span data-stu-id="e00d8-700">Component</span></span>

* <span data-ttu-id="e00d8-701">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-701">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-702">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-702">Monitor</span></span>

* <span data-ttu-id="e00d8-703">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-703">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-704">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-704">Resource</span></span>

* <span data-ttu-id="e00d8-705">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-705">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e00d8-706">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="e00d8-706">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-707">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-707">VM</span></span>

* <span data-ttu-id="e00d8-708">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-708">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e00d8-709">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-709">October 9, 2017</span></span>

<span data-ttu-id="e00d8-710">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e00d8-710">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-711">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-711">Core</span></span>

* <span data-ttu-id="e00d8-712">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-712">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-713">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-713">Appservice</span></span>

* <span data-ttu-id="e00d8-714">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-714">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e00d8-715">Batch</span><span class="sxs-lookup"><span data-stu-id="e00d8-715">Batch</span></span>

* <span data-ttu-id="e00d8-716">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e00d8-716">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e00d8-717">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-717">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e00d8-718">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-718">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e00d8-719">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-719">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e00d8-720">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e00d8-720">Batchai</span></span>

* <span data-ttu-id="e00d8-721">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-721">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00d8-722">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00d8-722">Keyvault</span></span>

* <span data-ttu-id="e00d8-723">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="e00d8-723">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e00d8-724">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e00d8-724">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e00d8-725">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-725">Network</span></span>

* <span data-ttu-id="e00d8-726">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="e00d8-726">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e00d8-727">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-727">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-728">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-728">Resource</span></span>

* <span data-ttu-id="e00d8-729">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-729">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e00d8-730">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-730">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e00d8-731">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-731">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e00d8-732">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-732">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-733">Sql</span><span class="sxs-lookup"><span data-stu-id="e00d8-733">Sql</span></span>

* <span data-ttu-id="e00d8-734">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-734">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e00d8-735">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-735">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e00d8-736">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-736">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-737">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-737">Storage</span></span>

* <span data-ttu-id="e00d8-738">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-738">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-739">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-739">Vm</span></span>

* <span data-ttu-id="e00d8-740">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="e00d8-740">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e00d8-741">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-741">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e00d8-742">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-742">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e00d8-743">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-743">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e00d8-744">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-744">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e00d8-745">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-745">September 22, 2017</span></span>

<span data-ttu-id="e00d8-746">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e00d8-746">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-747">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-747">Resource</span></span>

* <span data-ttu-id="e00d8-748">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-748">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e00d8-749">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-749">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e00d8-750">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-750">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e00d8-751">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="e00d8-751">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-752">Network</span></span>

* <span data-ttu-id="e00d8-753">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-753">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e00d8-754">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-754">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e00d8-755">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-755">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e00d8-756">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-756">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e00d8-757">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-757">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e00d8-758">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-758">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e00d8-759">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-759">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-760">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-760">Storage</span></span>

* <span data-ttu-id="e00d8-761">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e00d8-761">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e00d8-762">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="e00d8-762">Eventgrid</span></span>

* <span data-ttu-id="e00d8-763">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-763">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-764">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-764">SQL</span></span>

* <span data-ttu-id="e00d8-765">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="e00d8-765">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e00d8-766">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e00d8-766">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e00d8-767">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-767">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00d8-768">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00d8-768">Keyvault</span></span>

* <span data-ttu-id="e00d8-769">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-769">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-770">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-770">VM</span></span>

* <span data-ttu-id="e00d8-771">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-771">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e00d8-772">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e00d8-772">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e00d8-773">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-773">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e00d8-774">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-774">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e00d8-775">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-775">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e00d8-776">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-776">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-777">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-777">ACS</span></span>

* <span data-ttu-id="e00d8-778">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-778">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-779">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-779">Appservice</span></span>

* <span data-ttu-id="e00d8-780">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e00d8-780">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e00d8-781">Backup</span><span class="sxs-lookup"><span data-stu-id="e00d8-781">Backup</span></span>

* <span data-ttu-id="e00d8-782">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e00d8-782">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e00d8-783">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-783">September 11, 2017</span></span>

<span data-ttu-id="e00d8-784">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e00d8-784">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e00d8-785">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-785">Core</span></span>

* <span data-ttu-id="e00d8-786">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="e00d8-786">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e00d8-787">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="e00d8-787">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-788">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-788">Acs</span></span>

* <span data-ttu-id="e00d8-789">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-789">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e00d8-790">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-790">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-791">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-791">Appservice</span></span>

* <span data-ttu-id="e00d8-792">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="e00d8-792">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e00d8-793">CDN</span><span class="sxs-lookup"><span data-stu-id="e00d8-793">CDN</span></span>

* <span data-ttu-id="e00d8-794">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e00d8-794">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e00d8-795">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e00d8-795">Extension</span></span>

* <span data-ttu-id="e00d8-796">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-796">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00d8-797">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00d8-797">Keyvault</span></span>

* <span data-ttu-id="e00d8-798">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="e00d8-798">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-799">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-799">Network</span></span>

* <span data-ttu-id="e00d8-800">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-800">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e00d8-801">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-801">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e00d8-802">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-802">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e00d8-803">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-803">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e00d8-804">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-804">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-805">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-805">Resource</span></span>

* <span data-ttu-id="e00d8-806">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="e00d8-806">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e00d8-807">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="e00d8-807">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e00d8-808">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="e00d8-808">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e00d8-809">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-809">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-810">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-810">SQL</span></span>

* <span data-ttu-id="e00d8-811">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-811">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-812">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-812">VM</span></span>

* <span data-ttu-id="e00d8-813">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-813">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e00d8-814">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="e00d8-814">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e00d8-815">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-815">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e00d8-816">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="e00d8-816">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e00d8-817">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="e00d8-817">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e00d8-818">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-818">August 31, 2017</span></span>

<span data-ttu-id="e00d8-819">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e00d8-819">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00d8-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00d8-820">Keyvault</span></span>

* <span data-ttu-id="e00d8-821">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="e00d8-821">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e00d8-822">Sf</span><span class="sxs-lookup"><span data-stu-id="e00d8-822">Sf</span></span>

* <span data-ttu-id="e00d8-823">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-823">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-824">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-824">Storage</span></span>

* <span data-ttu-id="e00d8-825">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="e00d8-825">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e00d8-826">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="e00d8-826">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e00d8-827">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-827">August 28, 2017</span></span>

<span data-ttu-id="e00d8-828">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e00d8-828">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e00d8-829">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="e00d8-829">CLI</span></span>

* <span data-ttu-id="e00d8-830">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-830">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-831">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-831">ACS</span></span>

* <span data-ttu-id="e00d8-832">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-832">Corrected preview regions</span></span>
* <span data-ttu-id="e00d8-833">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-833">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e00d8-834">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-834">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-835">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-835">Appservice</span></span>

* <span data-ttu-id="e00d8-836">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-836">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e00d8-837">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-837">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e00d8-838">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-838">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e00d8-839">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="e00d8-839">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e00d8-840">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-840">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e00d8-841">IoT</span><span class="sxs-lookup"><span data-stu-id="e00d8-841">IoT</span></span>

* <span data-ttu-id="e00d8-842">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="e00d8-842">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-843">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-843">Network</span></span>

* <span data-ttu-id="e00d8-844">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-844">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e00d8-845">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-845">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e00d8-846">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-846">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e00d8-847">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-847">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e00d8-848">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-848">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-849">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-849">Profile</span></span>

* <span data-ttu-id="e00d8-850">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-850">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00d8-851">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00d8-851">Service Fabric</span></span>

* <span data-ttu-id="e00d8-852">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e00d8-852">Preview release</span></span>
* <span data-ttu-id="e00d8-853">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-853">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e00d8-854">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-854">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e00d8-855">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-855">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-856">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-856">Storage</span></span>

* <span data-ttu-id="e00d8-857">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-857">Enabled setting blob tier</span></span>
* <span data-ttu-id="e00d8-858">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-858">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e00d8-859">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-859">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e00d8-860">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-860">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e00d8-861">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-861">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e00d8-862">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="e00d8-862">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-863">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-863">VM</span></span>

* <span data-ttu-id="e00d8-864">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-864">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e00d8-865">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e00d8-865">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e00d8-866">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-866">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00d8-867">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="e00d8-867">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e00d8-868">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-868">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e00d8-869">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e00d8-869">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e00d8-870">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-870">August 15, 2017</span></span>

<span data-ttu-id="e00d8-871">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e00d8-871">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-872">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-872">ACS</span></span>

* <span data-ttu-id="e00d8-873">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-873">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-874">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-874">Appservice</span></span>

* <span data-ttu-id="e00d8-875">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-875">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00d8-876">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e00d8-876">Event Grid</span></span>

* <span data-ttu-id="e00d8-877">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-877">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e00d8-878">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-878">August 11, 2017</span></span>

<span data-ttu-id="e00d8-879">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e00d8-879">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-880">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-880">ACS</span></span>

* <span data-ttu-id="e00d8-881">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-881">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e00d8-882">Batch</span><span class="sxs-lookup"><span data-stu-id="e00d8-882">Batch</span></span>

* <span data-ttu-id="e00d8-883">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-883">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e00d8-884">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-884">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e00d8-885">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-885">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e00d8-886">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="e00d8-886">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e00d8-887">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="e00d8-887">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e00d8-888">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-888">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e00d8-889">Komponente</span><span class="sxs-lookup"><span data-stu-id="e00d8-889">Component</span></span>

* <span data-ttu-id="e00d8-890">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-890">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e00d8-891">Container</span><span class="sxs-lookup"><span data-stu-id="e00d8-891">Container</span></span>

* <span data-ttu-id="e00d8-892">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="e00d8-892">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e00d8-893">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00d8-893">Data Lake Store</span></span>

* <span data-ttu-id="e00d8-894">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-894">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00d8-895">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e00d8-895">Event Grid</span></span>

* <span data-ttu-id="e00d8-896">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e00d8-896">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-897">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-897">Network</span></span>

* <span data-ttu-id="e00d8-898">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-898">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e00d8-899">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="e00d8-899">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e00d8-900">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="e00d8-900">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e00d8-901">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e00d8-901">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-902">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-902">Profile</span></span>

* <span data-ttu-id="e00d8-903">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="e00d8-903">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-904">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-904">Storage</span></span>

* <span data-ttu-id="e00d8-905">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-905">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-906">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-906">VM</span></span>

* <span data-ttu-id="e00d8-907">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-907">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e00d8-908">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-908">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e00d8-909">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-909">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e00d8-910">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="e00d8-910">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e00d8-911">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-911">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e00d8-912">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-912">July 28, 2017</span></span>

<span data-ttu-id="e00d8-913">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e00d8-913">Version 2.0.12</span></span>

* <span data-ttu-id="e00d8-914">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-914">Added container commands</span></span>
* <span data-ttu-id="e00d8-915">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-915">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e00d8-916">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-916">Core</span></span>

* <span data-ttu-id="e00d8-917">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="e00d8-917">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e00d8-918">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-918">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e00d8-919">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="e00d8-919">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e00d8-920">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="e00d8-920">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e00d8-921">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="e00d8-921">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e00d8-922">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="e00d8-922">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e00d8-923">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="e00d8-923">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e00d8-924">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="e00d8-924">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e00d8-925">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="e00d8-925">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e00d8-926">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-926">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e00d8-927">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="e00d8-927">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e00d8-928">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="e00d8-928">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e00d8-929">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="e00d8-929">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e00d8-930">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="e00d8-930">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e00d8-931">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e00d8-931">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e00d8-932">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="e00d8-932">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e00d8-933">ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-933">ACR</span></span>

* <span data-ttu-id="e00d8-934">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-934">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e00d8-935">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-935">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e00d8-936">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-936">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e00d8-937">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-937">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e00d8-938">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-938">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e00d8-939">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-939">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-940">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-940">ACS</span></span>

* <span data-ttu-id="e00d8-941">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e00d8-941">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-942">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-942">Appservice</span></span>

* <span data-ttu-id="e00d8-943">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="e00d8-943">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e00d8-944">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="e00d8-944">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e00d8-945">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e00d8-945">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e00d8-946">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="e00d8-946">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e00d8-947">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="e00d8-947">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e00d8-948">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="e00d8-948">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e00d8-949">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="e00d8-949">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e00d8-950">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="e00d8-950">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e00d8-951">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-951">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e00d8-952">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="e00d8-952">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e00d8-953">Batch</span><span class="sxs-lookup"><span data-stu-id="e00d8-953">Batch</span></span>

* <span data-ttu-id="e00d8-954">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-954">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e00d8-955">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-955">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e00d8-956">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-956">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e00d8-957">CDN</span><span class="sxs-lookup"><span data-stu-id="e00d8-957">CDN</span></span>

* <span data-ttu-id="e00d8-958">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-958">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e00d8-959">Cloud</span><span class="sxs-lookup"><span data-stu-id="e00d8-959">Cloud</span></span>

* <span data-ttu-id="e00d8-960">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="e00d8-960">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e00d8-961">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="e00d8-961">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e00d8-962">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="e00d8-962">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e00d8-963">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="e00d8-963">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e00d8-964">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e00d8-964">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00d8-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00d8-965">CosmosDB</span></span>

* <span data-ttu-id="e00d8-966">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="e00d8-966">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e00d8-967">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-967">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00d8-968">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00d8-968">Data Lake Analytics</span></span>

* <span data-ttu-id="e00d8-969">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-969">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e00d8-970">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-970">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e00d8-971">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-971">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00d8-972">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00d8-972">Data Lake Store</span></span>

* <span data-ttu-id="e00d8-973">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-973">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e00d8-974">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="e00d8-974">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e00d8-975">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-975">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e00d8-976">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e00d8-976">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e00d8-977">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="e00d8-977">Interactive</span></span>

* <span data-ttu-id="e00d8-978">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-978">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e00d8-979">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-979">Increased test coverage</span></span>
* <span data-ttu-id="e00d8-980">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-980">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e00d8-981">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="e00d8-981">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e00d8-982">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="e00d8-982">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e00d8-983">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="e00d8-983">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e00d8-984">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="e00d8-984">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e00d8-985">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-985">Added `--progress` flag</span></span>
* <span data-ttu-id="e00d8-986">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-986">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e00d8-987">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="e00d8-987">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e00d8-988">IoT</span><span class="sxs-lookup"><span data-stu-id="e00d8-988">IoT</span></span>

* <span data-ttu-id="e00d8-989">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="e00d8-989">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e00d8-990">(3934)</span><span class="sxs-lookup"><span data-stu-id="e00d8-990">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e00d8-991">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="e00d8-991">Key vault</span></span>

* <span data-ttu-id="e00d8-992">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e00d8-992">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e00d8-993">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e00d8-993">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e00d8-994">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e00d8-994">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e00d8-995">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e00d8-995">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e00d8-996">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e00d8-996">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e00d8-997">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="e00d8-997">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e00d8-998">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-998">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e00d8-999">(3307)</span><span class="sxs-lookup"><span data-stu-id="e00d8-999">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e00d8-1000">Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-1000">Lab</span></span>

* <span data-ttu-id="e00d8-1001">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1001">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e00d8-1002">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1002">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-1003">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1003">Monitor</span></span>

* <span data-ttu-id="e00d8-1004">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1004">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e00d8-1005">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1005">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e00d8-1006">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1006">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e00d8-1007">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1007">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e00d8-1008">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1008">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e00d8-1009">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="e00d8-1009">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e00d8-1010">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1010">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e00d8-1011">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1011">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e00d8-1012">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="e00d8-1012">`location` no longer required</span></span>
  * <span data-ttu-id="e00d8-1013">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="e00d8-1013">Add name and ID support for target</span></span>
  * <span data-ttu-id="e00d8-1014">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1014">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e00d8-1015">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1015">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e00d8-1016">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1016">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e00d8-1017">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="e00d8-1017">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e00d8-1018">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1018">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e00d8-1019">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1019">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-1020">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-1020">Network</span></span>

* <span data-ttu-id="e00d8-1021">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1021">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e00d8-1022">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1022">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e00d8-1023">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e00d8-1023">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e00d8-1024">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e00d8-1024">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e00d8-1025">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-1025">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e00d8-1026">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1026">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e00d8-1027">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1027">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e00d8-1028">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1028">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e00d8-1029">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1029">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e00d8-1030">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1030">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e00d8-1031">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1031">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e00d8-1032">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1032">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e00d8-1033">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1033">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e00d8-1034">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1034">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e00d8-1035">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1035">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e00d8-1036">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1036">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e00d8-1037">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1037">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e00d8-1038">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="e00d8-1038">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e00d8-1039">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1039">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e00d8-1040">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-1040">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e00d8-1041">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="e00d8-1041">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e00d8-1042">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e00d8-1042">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e00d8-1043">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-1043">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e00d8-1044">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1044">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e00d8-1045">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1045">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e00d8-1046">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1046">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e00d8-1047">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1047">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-1048">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-1048">Profile</span></span>

* <span data-ttu-id="e00d8-1049">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="e00d8-1049">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e00d8-1050">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="e00d8-1050">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e00d8-1051">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1051">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e00d8-1052">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1052">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e00d8-1053">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="e00d8-1053">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00d8-1054">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00d8-1054">RDBMS</span></span>

* <span data-ttu-id="e00d8-1055">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1055">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e00d8-1056">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1056">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e00d8-1057">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1057">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e00d8-1058">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1058">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-1059">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-1059">Resource</span></span>

* <span data-ttu-id="e00d8-1060">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-1060">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e00d8-1061">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="e00d8-1061">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e00d8-1062">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-1062">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e00d8-1063">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1063">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e00d8-1064">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1064">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e00d8-1065">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-1065">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e00d8-1066">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1066">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e00d8-1067">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1067">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-1068">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-1068">Role</span></span>

* <span data-ttu-id="e00d8-1069">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1069">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e00d8-1070">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1070">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e00d8-1071">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="e00d8-1071">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e00d8-1072">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1072">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e00d8-1073">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1073">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00d8-1074">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00d8-1074">Service Fabric</span></span>
* <span data-ttu-id="e00d8-1075">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1075">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e00d8-1076">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1076">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e00d8-1077">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1077">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-1078">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-1078">SQL</span></span>

* <span data-ttu-id="e00d8-1079">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1079">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e00d8-1080">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1080">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e00d8-1081">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1081">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-1082">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-1082">Storage</span></span>

* <span data-ttu-id="e00d8-1083">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1083">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e00d8-1084">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-1084">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e00d8-1085">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1085">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e00d8-1086">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1086">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e00d8-1087">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1087">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e00d8-1088">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1088">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-1089">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-1089">VM</span></span>

* <span data-ttu-id="e00d8-1090">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="e00d8-1090">Support configuring nsg</span></span>
* <span data-ttu-id="e00d8-1091">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="e00d8-1091">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e00d8-1092">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="e00d8-1092">Support managed service identities</span></span>
* <span data-ttu-id="e00d8-1093">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="e00d8-1093">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e00d8-1094">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1094">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e00d8-1095">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-1095">May 10, 2017</span></span>

<span data-ttu-id="e00d8-1096">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e00d8-1096">Version 2.0.6</span></span>

* <span data-ttu-id="e00d8-1097">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1097">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e00d8-1098">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1098">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e00d8-1099">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="e00d8-1099">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e00d8-1100">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1100">Include Cognitive Services module</span></span>
* <span data-ttu-id="e00d8-1101">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1101">Include Service Fabric module</span></span>
* <span data-ttu-id="e00d8-1102">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1102">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e00d8-1103">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="e00d8-1103">Add support for CDN commands</span></span>
* <span data-ttu-id="e00d8-1104">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1104">Remove Container module</span></span>
* <span data-ttu-id="e00d8-1105">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1105">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e00d8-1106">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1106">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e00d8-1107">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-1107">Core</span></span>

* <span data-ttu-id="e00d8-1108">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1108">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e00d8-1109">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1109">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e00d8-1110">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1110">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e00d8-1111">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1111">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e00d8-1112">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1112">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e00d8-1113">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1113">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e00d8-1114">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1114">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e00d8-1115">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1115">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e00d8-1116">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1116">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e00d8-1117">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1117">core: Improved performance</span></span>
* <span data-ttu-id="e00d8-1118">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1118">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e00d8-1119">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-1119">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-1120">ACS</span></span>

* <span data-ttu-id="e00d8-1121">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e00d8-1121">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e00d8-1122">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1122">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e00d8-1123">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1123">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e00d8-1124">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1124">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-1125">AppService</span></span>

* <span data-ttu-id="e00d8-1126">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1126">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e00d8-1127">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1127">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e00d8-1128">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1128">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e00d8-1129">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="e00d8-1129">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e00d8-1130">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1130">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e00d8-1131">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1131">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e00d8-1132">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="e00d8-1132">support slot swap with preview</span></span>
* <span data-ttu-id="e00d8-1133">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1133">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e00d8-1134">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1134">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00d8-1135">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00d8-1135">CosmosDB</span></span>

* <span data-ttu-id="e00d8-1136">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e00d8-1136">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e00d8-1137">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1137">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e00d8-1138">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="e00d8-1138">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e00d8-1139">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="e00d8-1139">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00d8-1140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00d8-1140">Data Lake Analytics</span></span>

* <span data-ttu-id="e00d8-1141">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="e00d8-1141">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e00d8-1142">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1142">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e00d8-1143">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1143">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e00d8-1144">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="e00d8-1144">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e00d8-1145">Table</span><span class="sxs-lookup"><span data-stu-id="e00d8-1145">Table</span></span>
  * <span data-ttu-id="e00d8-1146">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="e00d8-1146">Table valued function</span></span>
  * <span data-ttu-id="e00d8-1147">Sicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-1147">View</span></span>
  * <span data-ttu-id="e00d8-1148">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1148">Table Statistics.</span></span> <span data-ttu-id="e00d8-1149">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1149">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00d8-1150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00d8-1150">Data Lake Store</span></span>

* <span data-ttu-id="e00d8-1151">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-1151">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e00d8-1152">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1152">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e00d8-1153">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="e00d8-1153">missed help for access show.</span></span> <span data-ttu-id="e00d8-1154">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e00d8-1154">adding it.</span></span> <span data-ttu-id="e00d8-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e00d8-1156">Suchen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1156">Find</span></span>

* <span data-ttu-id="e00d8-1157">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="e00d8-1157">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00d8-1158">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00d8-1158">KeyVault</span></span>

* <span data-ttu-id="e00d8-1159">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1159">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e00d8-1160">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="e00d8-1160">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e00d8-1161">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="e00d8-1161">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e00d8-1162">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="e00d8-1162">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e00d8-1163">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1163">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e00d8-1164">Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-1164">Lab</span></span>

* <span data-ttu-id="e00d8-1165">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="e00d8-1165">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e00d8-1166">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-1166">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e00d8-1167">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="e00d8-1167">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e00d8-1168">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="e00d8-1168">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e00d8-1169">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="e00d8-1169">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e00d8-1170">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1170">Monitor</span></span>

* <span data-ttu-id="e00d8-1171">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1171">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e00d8-1172">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1172">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e00d8-1173">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-1173">Network</span></span>

* <span data-ttu-id="e00d8-1174">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1174">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e00d8-1175">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1175">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e00d8-1176">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="e00d8-1176">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e00d8-1177">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1177">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e00d8-1178">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="e00d8-1178">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e00d8-1179">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="e00d8-1179">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e00d8-1180">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1180">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e00d8-1181">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1181">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e00d8-1182">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1182">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e00d8-1183">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="e00d8-1183">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e00d8-1184">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1184">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e00d8-1185">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1185">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e00d8-1186">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="e00d8-1186">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e00d8-1187">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e00d8-1187">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e00d8-1188">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e00d8-1188">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e00d8-1189">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1189">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e00d8-1190">Profil</span><span class="sxs-lookup"><span data-stu-id="e00d8-1190">Profile</span></span>

* <span data-ttu-id="e00d8-1191">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1191">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e00d8-1192">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1192">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e00d8-1193">Redis</span><span class="sxs-lookup"><span data-stu-id="e00d8-1193">Redis</span></span>

* <span data-ttu-id="e00d8-1194">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-1194">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e00d8-1195">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1195">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e00d8-1196">Ressource</span><span class="sxs-lookup"><span data-stu-id="e00d8-1196">Resource</span></span>

* <span data-ttu-id="e00d8-1197">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1197">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e00d8-1198">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1198">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e00d8-1199">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1199">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e00d8-1200">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="e00d8-1200">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e00d8-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e00d8-1202">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1202">Add docs for az lock update.</span></span> <span data-ttu-id="e00d8-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e00d8-1204">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="e00d8-1204">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e00d8-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e00d8-1206">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="e00d8-1206">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e00d8-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e00d8-1208">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1208">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e00d8-1209">Rolle</span><span class="sxs-lookup"><span data-stu-id="e00d8-1209">Role</span></span>

* <span data-ttu-id="e00d8-1210">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1210">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e00d8-1211">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1211">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e00d8-1212">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1212">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e00d8-1213">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="e00d8-1213">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e00d8-1214">SQL</span><span class="sxs-lookup"><span data-stu-id="e00d8-1214">SQL</span></span>

* <span data-ttu-id="e00d8-1215">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1215">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e00d8-1216">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1216">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e00d8-1217">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-1217">Storage</span></span>

* <span data-ttu-id="e00d8-1218">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1218">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e00d8-1219">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="e00d8-1219">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e00d8-1220">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="e00d8-1220">Add support for large block blob upload</span></span>
* <span data-ttu-id="e00d8-1221">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="e00d8-1221">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-1222">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-1222">VM</span></span>

* <span data-ttu-id="e00d8-1223">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="e00d8-1223">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e00d8-1224">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="e00d8-1224">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e00d8-1225">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e00d8-1225">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e00d8-1226">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e00d8-1226">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e00d8-1227">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1227">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e00d8-1228">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="e00d8-1228">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e00d8-1229">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1229">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e00d8-1230">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-1230">April 3, 2017</span></span>

<span data-ttu-id="e00d8-1231">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e00d8-1231">Version 2.0.2</span></span>

<span data-ttu-id="e00d8-1232">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1232">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e00d8-1233">Core</span><span class="sxs-lookup"><span data-stu-id="e00d8-1233">Core</span></span>

* <span data-ttu-id="e00d8-1234">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="e00d8-1234">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e00d8-1235">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1235">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e00d8-1236">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1236">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e00d8-1237">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1237">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e00d8-1238">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1238">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e00d8-1239">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="e00d8-1239">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e00d8-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e00d8-1241">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-1241">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e00d8-1242">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="e00d8-1242">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e00d8-1243">ACS</span><span class="sxs-lookup"><span data-stu-id="e00d8-1243">ACS</span></span>

* <span data-ttu-id="e00d8-1244">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1244">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e00d8-1245">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="e00d8-1245">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e00d8-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e00d8-1247">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="e00d8-1247">Add support for windows clusters.</span></span> <span data-ttu-id="e00d8-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e00d8-1249">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="e00d8-1249">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e00d8-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e00d8-1251">AppService</span><span class="sxs-lookup"><span data-stu-id="e00d8-1251">AppService</span></span>

* <span data-ttu-id="e00d8-1252">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1252">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e00d8-1253">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1253">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e00d8-1254">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1254">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e00d8-1255">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1255">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e00d8-1256">DataLake</span><span class="sxs-lookup"><span data-stu-id="e00d8-1256">DataLake</span></span>

* <span data-ttu-id="e00d8-1257">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1257">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e00d8-1258">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="e00d8-1258">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e00d8-1259">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e00d8-1259">DocuemntDB</span></span>

* <span data-ttu-id="e00d8-1260">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1260">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e00d8-1261">VM</span><span class="sxs-lookup"><span data-stu-id="e00d8-1261">VM</span></span>

* <span data-ttu-id="e00d8-1262">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1262">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e00d8-1263">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1263">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e00d8-1264">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1264">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e00d8-1265">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1265">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e00d8-1266">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1266">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e00d8-1267">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1267">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e00d8-1268">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e00d8-1268">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e00d8-1269">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="e00d8-1269">February 27, 2017</span></span>

<span data-ttu-id="e00d8-1270">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e00d8-1270">Version 2.0.0</span></span>

<span data-ttu-id="e00d8-1271">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="e00d8-1271">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e00d8-1272">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1272">Container Service (acs)</span></span>
- <span data-ttu-id="e00d8-1273">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1273">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e00d8-1274">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e00d8-1274">Networking</span></span>
- <span data-ttu-id="e00d8-1275">Speicher</span><span class="sxs-lookup"><span data-stu-id="e00d8-1275">Storage</span></span>

<span data-ttu-id="e00d8-1276">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1276">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e00d8-1277">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1277">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e00d8-1278">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1278">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e00d8-1279">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="e00d8-1279">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e00d8-1280">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="e00d8-1280">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e00d8-1281">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="e00d8-1281">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e00d8-1282">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1282">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e00d8-1283">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e00d8-1283">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e00d8-1284">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e00d8-1284">Provide feedback from the command line with the `az feedback` command</span></span>

