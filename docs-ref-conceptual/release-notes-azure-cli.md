---
title: Azure CLI 2.0-Versionshinweise
description: Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="999db-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="999db-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="999db-104">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="999db-104">March 27, 2018</span></span>

<span data-ttu-id="999db-105">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="999db-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="999db-106">Core</span><span class="sxs-lookup"><span data-stu-id="999db-106">Core</span></span>

* <span data-ttu-id="999db-107">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="999db-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="999db-108">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-108">ACS</span></span>

* <span data-ttu-id="999db-109">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="999db-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-110">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-110">Appservice</span></span>

* <span data-ttu-id="999db-111">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="999db-112">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="999db-113">Sicherung</span><span class="sxs-lookup"><span data-stu-id="999db-113">Backup</span></span>

* <span data-ttu-id="999db-114">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="999db-115">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="999db-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="999db-116">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="999db-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="999db-117">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="999db-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="999db-118">Container</span><span class="sxs-lookup"><span data-stu-id="999db-118">Container</span></span>

* <span data-ttu-id="999db-119">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-119">Added `container exec` command.</span></span> <span data-ttu-id="999db-120">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="999db-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="999db-121">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="999db-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="999db-122">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="999db-122">Extension</span></span>

* <span data-ttu-id="999db-123">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="999db-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="999db-124">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="999db-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="999db-125">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="999db-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="999db-126">Interactive</span></span>

* <span data-ttu-id="999db-127">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="999db-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="999db-128">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="999db-129">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="999db-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="999db-130">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="999db-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="999db-131">Labor</span><span class="sxs-lookup"><span data-stu-id="999db-131">Lab</span></span>

* <span data-ttu-id="999db-132">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-133">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-133">Monitor</span></span>

* <span data-ttu-id="999db-134">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="999db-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="999db-135">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="999db-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="999db-136">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="999db-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="999db-137">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-137">Network</span></span>

* <span data-ttu-id="999db-138">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="999db-139">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-139">Profile</span></span>

* <span data-ttu-id="999db-140">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="999db-141">RDBMS</span><span class="sxs-lookup"><span data-stu-id="999db-141">RDBMS</span></span>

* <span data-ttu-id="999db-142">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="999db-143">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-143">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="999db-145">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-145">Role</span></span>

* <span data-ttu-id="999db-146">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="999db-147">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="999db-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="999db-148">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="999db-149">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="999db-150">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="999db-151">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-151">Storage</span></span>

* <span data-ttu-id="999db-152">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="999db-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="999db-153">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="999db-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="999db-154">VM</span><span class="sxs-lookup"><span data-stu-id="999db-154">VM</span></span>

* <span data-ttu-id="999db-155">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="999db-156">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="999db-157">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="999db-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="999db-158">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="999db-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="999db-159">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="999db-159">March 13, 2018</span></span>

<span data-ttu-id="999db-160">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="999db-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="999db-161">ACR</span><span class="sxs-lookup"><span data-stu-id="999db-161">ACR</span></span>

* <span data-ttu-id="999db-162">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="999db-163">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="999db-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="999db-164">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="999db-165">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-165">ACS</span></span>

* <span data-ttu-id="999db-166">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="999db-167">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="999db-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="999db-168">Advisor</span><span class="sxs-lookup"><span data-stu-id="999db-168">Advisor</span></span>

* <span data-ttu-id="999db-169">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="999db-170">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="999db-171">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="999db-172">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="999db-173">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-174">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-174">Appservice</span></span>

* <span data-ttu-id="999db-175">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="999db-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="999db-176">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="999db-177">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="999db-177">Eventhubs</span></span>

* <span data-ttu-id="999db-178">Erste Version</span><span class="sxs-lookup"><span data-stu-id="999db-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="999db-179">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="999db-179">Extension</span></span>

* <span data-ttu-id="999db-180">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="999db-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-181">Interactive</span><span class="sxs-lookup"><span data-stu-id="999db-181">Interactive</span></span>

* <span data-ttu-id="999db-182">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="999db-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="999db-183">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="999db-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="999db-184">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="999db-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="999db-185">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-186">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-186">Monitor</span></span>

* <span data-ttu-id="999db-187">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="999db-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="999db-188">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="999db-189">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="999db-190">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="999db-191">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-191">Network</span></span>

* <span data-ttu-id="999db-192">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="999db-193">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="999db-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="999db-194">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="999db-195">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="999db-196">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-196">Profile</span></span>

* <span data-ttu-id="999db-197">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="999db-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="999db-198">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="999db-199">RDBMS</span><span class="sxs-lookup"><span data-stu-id="999db-199">RDBMS</span></span>

* <span data-ttu-id="999db-200">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="999db-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="999db-201">SERVICE BUS</span><span class="sxs-lookup"><span data-stu-id="999db-201">Service Bus</span></span>

* <span data-ttu-id="999db-202">Erste Version</span><span class="sxs-lookup"><span data-stu-id="999db-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="999db-203">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-203">Storage</span></span>

* <span data-ttu-id="999db-204">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="999db-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="999db-205">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="999db-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="999db-206">VM</span><span class="sxs-lookup"><span data-stu-id="999db-206">VM</span></span>

* <span data-ttu-id="999db-207">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="999db-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="999db-208">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="999db-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="999db-209">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="999db-210">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="999db-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="999db-211">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="999db-211">February 27, 2018</span></span>

<span data-ttu-id="999db-212">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="999db-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="999db-213">Core</span><span class="sxs-lookup"><span data-stu-id="999db-213">Core</span></span>

* <span data-ttu-id="999db-214">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="999db-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="999db-215">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="999db-216">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="999db-217">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-217">ACS</span></span>

* <span data-ttu-id="999db-218">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="999db-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="999db-219">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="999db-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="999db-220">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="999db-221">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-222">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-222">Appservice</span></span>

* <span data-ttu-id="999db-223">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="999db-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="999db-224">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="999db-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="999db-225">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="999db-225">Cognitive Services</span></span>

* <span data-ttu-id="999db-226">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="999db-227">Nutzung</span><span class="sxs-lookup"><span data-stu-id="999db-227">Consumption</span></span>

* <span data-ttu-id="999db-228">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="999db-229">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="999db-230">Container</span><span class="sxs-lookup"><span data-stu-id="999db-230">Container</span></span>

* <span data-ttu-id="999db-231">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="999db-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="999db-232">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-232">Network</span></span>

* <span data-ttu-id="999db-233">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="999db-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="999db-234">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-234">Resource</span></span>

* <span data-ttu-id="999db-235">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="999db-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="999db-236">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-236">Role</span></span>

* <span data-ttu-id="999db-237">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="999db-238">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-238">SQL</span></span>

* <span data-ttu-id="999db-239">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="999db-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="999db-240">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-240">Storage</span></span>

* <span data-ttu-id="999db-241">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="999db-242">VM</span><span class="sxs-lookup"><span data-stu-id="999db-242">VM</span></span>

* <span data-ttu-id="999db-243">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="999db-244">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="999db-244">February 13, 2018</span></span>

<span data-ttu-id="999db-245">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="999db-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="999db-246">Core</span><span class="sxs-lookup"><span data-stu-id="999db-246">Core</span></span>

* <span data-ttu-id="999db-247">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="999db-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="999db-248">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-248">ACS</span></span>

* <span data-ttu-id="999db-249">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="999db-250">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="999db-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="999db-251">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="999db-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="999db-252">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="999db-253">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="999db-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="999db-254">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="999db-255">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="999db-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="999db-256">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="999db-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-257">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-257">Appservice</span></span>

* <span data-ttu-id="999db-258">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="999db-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="999db-259">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="999db-260">CDN</span><span class="sxs-lookup"><span data-stu-id="999db-260">CDN</span></span>

* <span data-ttu-id="999db-261">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="999db-262">Container</span><span class="sxs-lookup"><span data-stu-id="999db-262">Container</span></span>

* <span data-ttu-id="999db-263">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="999db-264">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="999db-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="999db-265">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="999db-265">CosmosDB</span></span>

* <span data-ttu-id="999db-266">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="999db-267">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="999db-267">Extension</span></span>

* <span data-ttu-id="999db-268">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="999db-269">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="999db-270">Feedback</span><span class="sxs-lookup"><span data-stu-id="999db-270">Feedback</span></span>

* <span data-ttu-id="999db-271">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="999db-272">Interactive</span></span>

* <span data-ttu-id="999db-273">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="999db-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="999db-274">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="999db-275">IoT</span><span class="sxs-lookup"><span data-stu-id="999db-275">IoT</span></span>

* <span data-ttu-id="999db-276">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="999db-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="999db-277">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="999db-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="999db-278">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="999db-279">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-280">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-280">Monitor</span></span>

* <span data-ttu-id="999db-281">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="999db-282">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-282">Network</span></span>

* <span data-ttu-id="999db-283">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="999db-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="999db-284">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-284">Profile</span></span>

* <span data-ttu-id="999db-285">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="999db-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="999db-286">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-286">Resource</span></span>

* <span data-ttu-id="999db-287">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="999db-288">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-288">Role</span></span>

* <span data-ttu-id="999db-289">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="999db-290">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-290">SQL</span></span>

* <span data-ttu-id="999db-291">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="999db-292">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-292">Added `sql db rename`</span></span>
* <span data-ttu-id="999db-293">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="999db-294">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-294">Storage</span></span>

* <span data-ttu-id="999db-295">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="999db-296">VM</span><span class="sxs-lookup"><span data-stu-id="999db-296">VM</span></span>

* <span data-ttu-id="999db-297">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="999db-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="999db-298">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="999db-299">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="999db-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="999db-300">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="999db-300">January 31, 2018</span></span>

<span data-ttu-id="999db-301">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="999db-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="999db-302">Core</span><span class="sxs-lookup"><span data-stu-id="999db-302">Core</span></span>

* <span data-ttu-id="999db-303">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="999db-304">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="999db-305">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="999db-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="999db-306">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="999db-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="999db-307">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="999db-308">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-308">ACS</span></span>

* <span data-ttu-id="999db-309">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="999db-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="999db-310">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-311">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-311">Appservice</span></span>

* <span data-ttu-id="999db-312">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="999db-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="999db-313">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="999db-314">CDN</span><span class="sxs-lookup"><span data-stu-id="999db-314">CDN</span></span>

* <span data-ttu-id="999db-315">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="999db-316">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="999db-316">CosmosDB</span></span>

* <span data-ttu-id="999db-317">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="999db-318">Interactive</span></span>

* <span data-ttu-id="999db-319">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="999db-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="999db-320">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-320">Network</span></span>

* <span data-ttu-id="999db-321">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="999db-322">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="999db-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="999db-323">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="999db-324">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="999db-325">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="999db-326">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="999db-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="999db-327">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="999db-328">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="999db-329">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="999db-330">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="999db-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="999db-331">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-331">Profile</span></span>

* <span data-ttu-id="999db-332">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="999db-333">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-333">Resource</span></span>

* <span data-ttu-id="999db-334">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="999db-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="999db-335">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-335">Storage</span></span>

* <span data-ttu-id="999db-336">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="999db-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="999db-337">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="999db-338">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="999db-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="999db-339">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="999db-340">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="999db-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="999db-341">VM</span><span class="sxs-lookup"><span data-stu-id="999db-341">VM</span></span>

* <span data-ttu-id="999db-342">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="999db-343">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="999db-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="999db-344">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="999db-345">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="999db-346">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="999db-346">January 17, 2018</span></span>

<span data-ttu-id="999db-347">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="999db-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="999db-348">ACR</span><span class="sxs-lookup"><span data-stu-id="999db-348">ACR</span></span>

* <span data-ttu-id="999db-349">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="999db-350">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="999db-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="999db-351">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-351">ACS</span></span>

* <span data-ttu-id="999db-352">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="999db-353">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-354">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-354">Appservice</span></span>

* <span data-ttu-id="999db-355">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="999db-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="999db-356">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="999db-357">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="999db-358">Sicherung</span><span class="sxs-lookup"><span data-stu-id="999db-358">Backup</span></span>

* <span data-ttu-id="999db-359">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="999db-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="999db-360">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="999db-361">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="999db-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="999db-362">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="999db-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="999db-363">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="999db-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="999db-364">Batch</span><span class="sxs-lookup"><span data-stu-id="999db-364">Batch</span></span>

* <span data-ttu-id="999db-365">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="999db-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="999db-366">Cloud</span><span class="sxs-lookup"><span data-stu-id="999db-366">Cloud</span></span>

* <span data-ttu-id="999db-367">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="999db-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="999db-368">Nutzung</span><span class="sxs-lookup"><span data-stu-id="999db-368">Consumption</span></span>

* <span data-ttu-id="999db-369">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="999db-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="999db-370">Event Grid</span><span class="sxs-lookup"><span data-stu-id="999db-370">Event Grid</span></span>

* <span data-ttu-id="999db-371">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="999db-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="999db-372">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="999db-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="999db-373">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="999db-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="999db-374">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="999db-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="999db-375">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="999db-376">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="999db-377">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="999db-378">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-379">Interactive</span><span class="sxs-lookup"><span data-stu-id="999db-379">Interactive</span></span>

* <span data-ttu-id="999db-380">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="999db-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="999db-381">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="999db-381">Fixed errors on startup</span></span>
* <span data-ttu-id="999db-382">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="999db-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="999db-383">IoT</span><span class="sxs-lookup"><span data-stu-id="999db-383">IoT</span></span>

* <span data-ttu-id="999db-384">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="999db-385">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="999db-386">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="999db-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-387">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-387">Monitor</span></span>

* <span data-ttu-id="999db-388">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="999db-389">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="999db-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="999db-390">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="999db-391">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-391">Network</span></span>

* <span data-ttu-id="999db-392">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="999db-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="999db-393">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="999db-394">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-394">Profile</span></span>

* <span data-ttu-id="999db-395">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="999db-396">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-396">Role</span></span>

* <span data-ttu-id="999db-397">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="999db-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="999db-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="999db-398">Service Fabric</span></span>

* <span data-ttu-id="999db-399">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="999db-400">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="999db-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="999db-401">VM</span><span class="sxs-lookup"><span data-stu-id="999db-401">VM</span></span>

* <span data-ttu-id="999db-402">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="999db-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="999db-403">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="999db-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="999db-404">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="999db-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="999db-405">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="999db-406">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="999db-407">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="999db-408">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="999db-409">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="999db-410">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="999db-410">December 19, 2017</span></span>

<span data-ttu-id="999db-411">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="999db-411">Version 2.0.23</span></span>

* <span data-ttu-id="999db-412">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="999db-413">Container</span><span class="sxs-lookup"><span data-stu-id="999db-413">Container</span></span>

* <span data-ttu-id="999db-414">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="999db-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="999db-415">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-415">Network</span></span>

* <span data-ttu-id="999db-416">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="999db-417">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="999db-418">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-418">Storage</span></span>

* <span data-ttu-id="999db-419">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="999db-420">VM</span><span class="sxs-lookup"><span data-stu-id="999db-420">VM</span></span>

* <span data-ttu-id="999db-421">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="999db-422">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="999db-422">December 5, 2017</span></span>

<span data-ttu-id="999db-423">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="999db-423">Version 2.0.22</span></span>

* <span data-ttu-id="999db-424">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="999db-424">Removed `az component` commands.</span></span> <span data-ttu-id="999db-425">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="999db-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="999db-426">Core</span><span class="sxs-lookup"><span data-stu-id="999db-426">Core</span></span>
* <span data-ttu-id="999db-427">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="999db-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="999db-428">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="999db-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="999db-429">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-429">ACS</span></span>

* <span data-ttu-id="999db-430">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="999db-431">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="999db-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="999db-432">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="999db-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="999db-433">Advisor</span><span class="sxs-lookup"><span data-stu-id="999db-433">Advisor</span></span>

* <span data-ttu-id="999db-434">Erste Version</span><span class="sxs-lookup"><span data-stu-id="999db-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-435">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-435">Appservice</span></span>

* <span data-ttu-id="999db-436">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="999db-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="999db-437">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="999db-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="999db-438">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="999db-439">Nutzung</span><span class="sxs-lookup"><span data-stu-id="999db-439">Consumption</span></span>

* <span data-ttu-id="999db-440">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="999db-441">Container</span><span class="sxs-lookup"><span data-stu-id="999db-441">Container</span></span>

* <span data-ttu-id="999db-442">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="999db-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-443">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-443">Monitor</span></span>

* <span data-ttu-id="999db-444">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="999db-445">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-445">Resource</span></span>

* <span data-ttu-id="999db-446">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="999db-447">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-447">Role</span></span>

* <span data-ttu-id="999db-448">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="999db-449">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="999db-450">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="999db-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="999db-451">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-451">SQL</span></span>

* <span data-ttu-id="999db-452">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="999db-453">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="999db-454">VM</span><span class="sxs-lookup"><span data-stu-id="999db-454">VM</span></span>

* <span data-ttu-id="999db-455">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="999db-456">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="999db-456">November 14, 2017</span></span>

<span data-ttu-id="999db-457">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="999db-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="999db-458">ACR</span><span class="sxs-lookup"><span data-stu-id="999db-458">ACR</span></span>

* <span data-ttu-id="999db-459">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="999db-460">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-460">ACS</span></span>

* <span data-ttu-id="999db-461">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="999db-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="999db-462">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="999db-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="999db-463">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="999db-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="999db-464">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="999db-465">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-466">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-466">Appservice</span></span>

* <span data-ttu-id="999db-467">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="999db-468">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="999db-469">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="999db-470">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="999db-471">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="999db-472">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="999db-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="999db-473">Batch</span><span class="sxs-lookup"><span data-stu-id="999db-473">Batch</span></span>

* <span data-ttu-id="999db-474">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="999db-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="999db-475">BatchAI</span><span class="sxs-lookup"><span data-stu-id="999db-475">Batchai</span></span>

* <span data-ttu-id="999db-476">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="999db-477">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="999db-478">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="999db-479">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="999db-480">Cloud</span><span class="sxs-lookup"><span data-stu-id="999db-480">Cloud</span></span>

* <span data-ttu-id="999db-481">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="999db-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="999db-482">Container</span><span class="sxs-lookup"><span data-stu-id="999db-482">Container</span></span>

* <span data-ttu-id="999db-483">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="999db-484">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-484">Added container group restart policy</span></span>
* <span data-ttu-id="999db-485">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="999db-486">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="999db-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="999db-487">Data Lake Analytics</span></span>

* <span data-ttu-id="999db-488">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="999db-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="999db-489">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-489">Data Lake Store</span></span>

* <span data-ttu-id="999db-490">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="999db-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="999db-491">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="999db-491">Extension</span></span>

* <span data-ttu-id="999db-492">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="999db-493">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="999db-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="999db-494">IoT</span><span class="sxs-lookup"><span data-stu-id="999db-494">IoT</span></span>

* <span data-ttu-id="999db-495">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-496">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-496">Monitor</span></span>

* <span data-ttu-id="999db-497">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="999db-498">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-498">Network</span></span>

* <span data-ttu-id="999db-499">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="999db-500">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="999db-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="999db-501">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="999db-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="999db-502">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="999db-503">Reservations</span><span class="sxs-lookup"><span data-stu-id="999db-503">Reservations</span></span>

* <span data-ttu-id="999db-504">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="999db-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="999db-505">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-505">Resource</span></span>

* <span data-ttu-id="999db-506">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="999db-507">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-507">SQL</span></span>

* <span data-ttu-id="999db-508">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="999db-509">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-509">Storage</span></span>

* <span data-ttu-id="999db-510">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="999db-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="999db-511">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="999db-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="999db-512">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="999db-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="999db-513">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="999db-514">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="999db-515">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="999db-516">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="999db-517">VM</span><span class="sxs-lookup"><span data-stu-id="999db-517">VM</span></span>

* <span data-ttu-id="999db-518">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="999db-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="999db-519">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="999db-520">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="999db-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="999db-521">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="999db-522">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="999db-523">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="999db-523">October 24, 2017</span></span>

<span data-ttu-id="999db-524">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="999db-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="999db-525">Core</span><span class="sxs-lookup"><span data-stu-id="999db-525">Core</span></span>

* <span data-ttu-id="999db-526">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="999db-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="999db-527">ACR</span><span class="sxs-lookup"><span data-stu-id="999db-527">ACR</span></span>

* <span data-ttu-id="999db-528">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="999db-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="999db-529">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="999db-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="999db-530">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="999db-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="999db-531">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-531">ACS</span></span>

* <span data-ttu-id="999db-532">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="999db-533">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="999db-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-534">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-534">Appservice</span></span>

* <span data-ttu-id="999db-535">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="999db-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="999db-536">Komponente</span><span class="sxs-lookup"><span data-stu-id="999db-536">Component</span></span>

* <span data-ttu-id="999db-537">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-538">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-538">Monitor</span></span>

* <span data-ttu-id="999db-539">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="999db-540">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-540">Resource</span></span>

* <span data-ttu-id="999db-541">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="999db-542">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="999db-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="999db-543">VM</span><span class="sxs-lookup"><span data-stu-id="999db-543">VM</span></span>

* <span data-ttu-id="999db-544">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="999db-545">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="999db-545">October 9, 2017</span></span>

<span data-ttu-id="999db-546">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="999db-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="999db-547">Core</span><span class="sxs-lookup"><span data-stu-id="999db-547">Core</span></span>

* <span data-ttu-id="999db-548">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-549">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-549">Appservice</span></span>

* <span data-ttu-id="999db-550">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="999db-551">Batch</span><span class="sxs-lookup"><span data-stu-id="999db-551">Batch</span></span>

* <span data-ttu-id="999db-552">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="999db-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="999db-553">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="999db-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="999db-554">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="999db-555">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="999db-556">BatchAI</span><span class="sxs-lookup"><span data-stu-id="999db-556">Batchai</span></span>

* <span data-ttu-id="999db-557">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="999db-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="999db-558">KeyVault</span><span class="sxs-lookup"><span data-stu-id="999db-558">Keyvault</span></span>

* <span data-ttu-id="999db-559">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="999db-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="999db-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="999db-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="999db-561">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-561">Network</span></span>

* <span data-ttu-id="999db-562">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="999db-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="999db-563">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="999db-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="999db-564">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-564">Resource</span></span>

* <span data-ttu-id="999db-565">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="999db-566">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="999db-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="999db-567">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="999db-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="999db-568">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="999db-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="999db-569">Sql</span><span class="sxs-lookup"><span data-stu-id="999db-569">Sql</span></span>

* <span data-ttu-id="999db-570">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="999db-571">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="999db-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="999db-572">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="999db-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="999db-573">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-573">Storage</span></span>

* <span data-ttu-id="999db-574">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="999db-575">VM</span><span class="sxs-lookup"><span data-stu-id="999db-575">Vm</span></span>

* <span data-ttu-id="999db-576">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="999db-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="999db-577">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="999db-578">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="999db-579">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="999db-580">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="999db-581">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="999db-581">September 22, 2017</span></span>

<span data-ttu-id="999db-582">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="999db-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="999db-583">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-583">Resource</span></span>

* <span data-ttu-id="999db-584">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="999db-585">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="999db-586">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="999db-587">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="999db-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="999db-588">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-588">Network</span></span>

* <span data-ttu-id="999db-589">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="999db-590">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="999db-591">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="999db-592">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="999db-593">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="999db-594">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="999db-595">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="999db-596">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-596">Storage</span></span>

* <span data-ttu-id="999db-597">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="999db-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="999db-598">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="999db-598">Eventgrid</span></span>

* <span data-ttu-id="999db-599">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="999db-600">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-600">SQL</span></span>

* <span data-ttu-id="999db-601">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="999db-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="999db-602">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="999db-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="999db-603">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="999db-604">KeyVault</span><span class="sxs-lookup"><span data-stu-id="999db-604">Keyvault</span></span>

* <span data-ttu-id="999db-605">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="999db-606">VM</span><span class="sxs-lookup"><span data-stu-id="999db-606">VM</span></span>

* <span data-ttu-id="999db-607">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="999db-608">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="999db-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="999db-609">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="999db-610">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="999db-611">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="999db-612">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="999db-613">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-613">ACS</span></span>

* <span data-ttu-id="999db-614">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-615">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-615">Appservice</span></span>

* <span data-ttu-id="999db-616">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="999db-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="999db-617">Sicherung</span><span class="sxs-lookup"><span data-stu-id="999db-617">Backup</span></span>

* <span data-ttu-id="999db-618">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="999db-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="999db-619">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="999db-619">September 11, 2017</span></span>

<span data-ttu-id="999db-620">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="999db-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="999db-621">Core</span><span class="sxs-lookup"><span data-stu-id="999db-621">Core</span></span>

* <span data-ttu-id="999db-622">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="999db-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="999db-623">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="999db-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="999db-624">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-624">Acs</span></span>

* <span data-ttu-id="999db-625">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="999db-626">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="999db-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-627">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-627">Appservice</span></span>

* <span data-ttu-id="999db-628">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="999db-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="999db-629">CDN</span><span class="sxs-lookup"><span data-stu-id="999db-629">CDN</span></span>

* <span data-ttu-id="999db-630">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="999db-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="999db-631">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="999db-631">Extension</span></span>

* <span data-ttu-id="999db-632">Erste Version</span><span class="sxs-lookup"><span data-stu-id="999db-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="999db-633">KeyVault</span><span class="sxs-lookup"><span data-stu-id="999db-633">Keyvault</span></span>

* <span data-ttu-id="999db-634">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="999db-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="999db-635">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-635">Network</span></span>

* <span data-ttu-id="999db-636">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="999db-637">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="999db-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="999db-638">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="999db-639">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="999db-640">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="999db-641">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-641">Resource</span></span>

* <span data-ttu-id="999db-642">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="999db-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="999db-643">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="999db-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="999db-644">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="999db-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="999db-645">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="999db-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="999db-646">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-646">SQL</span></span>

* <span data-ttu-id="999db-647">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="999db-648">VM</span><span class="sxs-lookup"><span data-stu-id="999db-648">VM</span></span>

* <span data-ttu-id="999db-649">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="999db-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="999db-650">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="999db-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="999db-651">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="999db-652">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="999db-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="999db-653">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="999db-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="999db-654">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="999db-654">August 31, 2017</span></span>

<span data-ttu-id="999db-655">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="999db-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="999db-656">KeyVault</span><span class="sxs-lookup"><span data-stu-id="999db-656">Keyvault</span></span>

* <span data-ttu-id="999db-657">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="999db-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="999db-658">Sf</span><span class="sxs-lookup"><span data-stu-id="999db-658">Sf</span></span>

* <span data-ttu-id="999db-659">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="999db-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="999db-660">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-660">Storage</span></span>

* <span data-ttu-id="999db-661">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="999db-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="999db-662">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="999db-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="999db-663">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="999db-663">August 28, 2017</span></span>

<span data-ttu-id="999db-664">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="999db-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="999db-665">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="999db-665">CLI</span></span>

* <span data-ttu-id="999db-666">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="999db-667">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-667">ACS</span></span>

* <span data-ttu-id="999db-668">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-668">Corrected preview regions</span></span>
* <span data-ttu-id="999db-669">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="999db-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="999db-670">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="999db-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-671">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-671">Appservice</span></span>

* <span data-ttu-id="999db-672">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="999db-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="999db-673">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="999db-674">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="999db-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="999db-675">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="999db-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="999db-676">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="999db-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="999db-677">IoT</span><span class="sxs-lookup"><span data-stu-id="999db-677">IoT</span></span>

* <span data-ttu-id="999db-678">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="999db-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="999db-679">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-679">Network</span></span>

* <span data-ttu-id="999db-680">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="999db-681">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="999db-682">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="999db-683">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="999db-684">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="999db-685">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-685">Profile</span></span>

* <span data-ttu-id="999db-686">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="999db-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="999db-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="999db-687">Service Fabric</span></span>

* <span data-ttu-id="999db-688">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="999db-688">Preview release</span></span>
* <span data-ttu-id="999db-689">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="999db-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="999db-690">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="999db-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="999db-691">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="999db-692">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-692">Storage</span></span>

* <span data-ttu-id="999db-693">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="999db-694">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="999db-695">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="999db-696">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="999db-697">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="999db-698">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="999db-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="999db-699">VM</span><span class="sxs-lookup"><span data-stu-id="999db-699">VM</span></span>

* <span data-ttu-id="999db-700">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="999db-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="999db-701">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="999db-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="999db-702">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="999db-703">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="999db-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="999db-704">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="999db-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="999db-705">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="999db-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="999db-706">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="999db-706">August 15, 2017</span></span>

<span data-ttu-id="999db-707">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="999db-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="999db-708">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-708">ACS</span></span>

* <span data-ttu-id="999db-709">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-710">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-710">Appservice</span></span>

* <span data-ttu-id="999db-711">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="999db-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="999db-712">Event Grid</span><span class="sxs-lookup"><span data-stu-id="999db-712">Event Grid</span></span>

* <span data-ttu-id="999db-713">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="999db-714">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="999db-714">August 11, 2017</span></span>

<span data-ttu-id="999db-715">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="999db-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="999db-716">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-716">ACS</span></span>

* <span data-ttu-id="999db-717">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="999db-718">Batch</span><span class="sxs-lookup"><span data-stu-id="999db-718">Batch</span></span>

* <span data-ttu-id="999db-719">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="999db-720">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="999db-721">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="999db-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="999db-722">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="999db-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="999db-723">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="999db-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="999db-724">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="999db-725">Komponente</span><span class="sxs-lookup"><span data-stu-id="999db-725">Component</span></span>

* <span data-ttu-id="999db-726">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="999db-727">Container</span><span class="sxs-lookup"><span data-stu-id="999db-727">Container</span></span>

* <span data-ttu-id="999db-728">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="999db-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="999db-729">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-729">Data Lake Store</span></span>

* <span data-ttu-id="999db-730">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="999db-731">Event Grid</span><span class="sxs-lookup"><span data-stu-id="999db-731">Event Grid</span></span>

* <span data-ttu-id="999db-732">Erste Version</span><span class="sxs-lookup"><span data-stu-id="999db-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="999db-733">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-733">Network</span></span>

* <span data-ttu-id="999db-734">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="999db-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="999db-735">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="999db-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="999db-736">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="999db-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="999db-737">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="999db-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="999db-738">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-738">Profile</span></span>

* <span data-ttu-id="999db-739">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="999db-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="999db-740">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-740">Storage</span></span>

* <span data-ttu-id="999db-741">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="999db-742">VM</span><span class="sxs-lookup"><span data-stu-id="999db-742">VM</span></span>

* <span data-ttu-id="999db-743">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="999db-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="999db-744">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="999db-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="999db-745">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="999db-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="999db-746">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="999db-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="999db-747">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="999db-748">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="999db-748">July 28, 2017</span></span>

<span data-ttu-id="999db-749">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="999db-749">Version 2.0.12</span></span>

* <span data-ttu-id="999db-750">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-750">Added container commands</span></span>
* <span data-ttu-id="999db-751">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-751">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="999db-752">Core</span><span class="sxs-lookup"><span data-stu-id="999db-752">Core</span></span>

* <span data-ttu-id="999db-753">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="999db-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="999db-754">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="999db-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="999db-755">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="999db-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="999db-756">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="999db-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="999db-757">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="999db-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="999db-758">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="999db-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="999db-759">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="999db-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="999db-760">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="999db-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="999db-761">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="999db-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="999db-762">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="999db-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="999db-763">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="999db-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="999db-764">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="999db-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="999db-765">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="999db-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="999db-766">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="999db-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="999db-767">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="999db-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="999db-768">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="999db-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="999db-769">ACR</span><span class="sxs-lookup"><span data-stu-id="999db-769">ACR</span></span>

* <span data-ttu-id="999db-770">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="999db-771">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="999db-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="999db-772">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="999db-773">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="999db-774">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="999db-775">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="999db-776">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-776">ACS</span></span>

* <span data-ttu-id="999db-777">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="999db-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-778">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-778">Appservice</span></span>

* <span data-ttu-id="999db-779">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="999db-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="999db-780">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="999db-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="999db-781">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="999db-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="999db-782">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="999db-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="999db-783">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="999db-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="999db-784">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="999db-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="999db-785">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="999db-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="999db-786">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="999db-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="999db-787">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="999db-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="999db-788">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="999db-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="999db-789">Batch</span><span class="sxs-lookup"><span data-stu-id="999db-789">Batch</span></span>

* <span data-ttu-id="999db-790">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="999db-791">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="999db-792">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="999db-793">CDN</span><span class="sxs-lookup"><span data-stu-id="999db-793">CDN</span></span>

* <span data-ttu-id="999db-794">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="999db-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="999db-795">Cloud</span><span class="sxs-lookup"><span data-stu-id="999db-795">Cloud</span></span>

* <span data-ttu-id="999db-796">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="999db-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="999db-797">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="999db-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="999db-798">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="999db-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="999db-799">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="999db-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="999db-800">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="999db-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="999db-801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="999db-801">CosmosDB</span></span>

* <span data-ttu-id="999db-802">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="999db-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="999db-803">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="999db-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="999db-804">Data Lake Analytics</span></span>

* <span data-ttu-id="999db-805">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="999db-806">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="999db-807">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="999db-808">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-808">Data Lake Store</span></span>

* <span data-ttu-id="999db-809">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="999db-810">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="999db-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="999db-811">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="999db-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="999db-812">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="999db-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="999db-813">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="999db-813">Interactive</span></span>

* <span data-ttu-id="999db-814">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="999db-815">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-815">Increased test coverage</span></span>
* <span data-ttu-id="999db-816">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="999db-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="999db-817">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="999db-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="999db-818">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="999db-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="999db-819">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="999db-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="999db-820">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="999db-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="999db-821">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-821">Added `--progress` flag</span></span>
* <span data-ttu-id="999db-822">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="999db-823">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="999db-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="999db-824">IoT</span><span class="sxs-lookup"><span data-stu-id="999db-824">IoT</span></span>

* <span data-ttu-id="999db-825">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="999db-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="999db-826">(3934)</span><span class="sxs-lookup"><span data-stu-id="999db-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="999db-827">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="999db-827">Key vault</span></span>

* <span data-ttu-id="999db-828">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="999db-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="999db-829">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="999db-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="999db-830">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="999db-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="999db-831">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="999db-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="999db-832">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="999db-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="999db-833">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="999db-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="999db-834">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="999db-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="999db-835">(3307)</span><span class="sxs-lookup"><span data-stu-id="999db-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="999db-836">Labor</span><span class="sxs-lookup"><span data-stu-id="999db-836">Lab</span></span>

* <span data-ttu-id="999db-837">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="999db-838">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-839">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-839">Monitor</span></span>

* <span data-ttu-id="999db-840">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="999db-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="999db-841">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="999db-842">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="999db-843">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="999db-844">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="999db-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="999db-845">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="999db-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="999db-846">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="999db-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="999db-847">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="999db-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="999db-848">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="999db-848">`location` no longer required</span></span>
  * <span data-ttu-id="999db-849">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="999db-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="999db-850">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="999db-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="999db-851">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="999db-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="999db-852">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="999db-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="999db-853">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="999db-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="999db-854">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="999db-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="999db-855">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="999db-856">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-856">Network</span></span>

* <span data-ttu-id="999db-857">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="999db-858">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="999db-859">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="999db-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="999db-860">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="999db-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="999db-861">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="999db-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="999db-862">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="999db-863">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="999db-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="999db-864">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="999db-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="999db-865">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="999db-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="999db-866">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="999db-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="999db-867">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="999db-868">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="999db-869">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="999db-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="999db-870">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="999db-871">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="999db-872">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="999db-873">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="999db-874">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="999db-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="999db-875">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="999db-876">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="999db-877">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="999db-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="999db-878">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="999db-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="999db-879">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="999db-880">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="999db-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="999db-881">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="999db-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="999db-882">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="999db-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="999db-883">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="999db-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="999db-884">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-884">Profile</span></span>

* <span data-ttu-id="999db-885">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="999db-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="999db-886">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="999db-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="999db-887">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="999db-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="999db-888">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="999db-889">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="999db-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="999db-890">RDBMS</span><span class="sxs-lookup"><span data-stu-id="999db-890">RDBMS</span></span>

* <span data-ttu-id="999db-891">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="999db-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="999db-892">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="999db-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="999db-893">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="999db-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="999db-894">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="999db-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="999db-895">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-895">Resource</span></span>

* <span data-ttu-id="999db-896">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="999db-897">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="999db-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="999db-898">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="999db-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="999db-899">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="999db-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="999db-900">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="999db-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="999db-901">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="999db-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="999db-902">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="999db-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="999db-903">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="999db-904">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-904">Role</span></span>

* <span data-ttu-id="999db-905">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="999db-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="999db-906">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="999db-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="999db-907">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="999db-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="999db-908">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="999db-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="999db-909">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="999db-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="999db-910">Service Fabric</span></span>
* <span data-ttu-id="999db-911">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="999db-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="999db-912">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="999db-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="999db-913">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="999db-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="999db-914">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-914">SQL</span></span>

* <span data-ttu-id="999db-915">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="999db-916">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="999db-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="999db-917">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="999db-918">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-918">Storage</span></span>

* <span data-ttu-id="999db-919">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="999db-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="999db-920">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="999db-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="999db-921">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="999db-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="999db-922">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="999db-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="999db-923">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="999db-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="999db-924">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="999db-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="999db-925">VM</span><span class="sxs-lookup"><span data-stu-id="999db-925">VM</span></span>

* <span data-ttu-id="999db-926">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="999db-926">Support configuring nsg</span></span>
* <span data-ttu-id="999db-927">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="999db-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="999db-928">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="999db-928">Support managed service identities</span></span>
* <span data-ttu-id="999db-929">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="999db-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="999db-930">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="999db-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="999db-931">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="999db-931">May 10, 2017</span></span>

<span data-ttu-id="999db-932">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="999db-932">Version 2.0.6</span></span>

* <span data-ttu-id="999db-933">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="999db-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="999db-934">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="999db-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="999db-935">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="999db-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="999db-936">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="999db-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="999db-937">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="999db-937">Include Service Fabric module</span></span>
* <span data-ttu-id="999db-938">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="999db-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="999db-939">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="999db-939">Add support for CDN commands</span></span>
* <span data-ttu-id="999db-940">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="999db-940">Remove Container module</span></span>
* <span data-ttu-id="999db-941">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="999db-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="999db-942">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="999db-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="999db-943">Core</span><span class="sxs-lookup"><span data-stu-id="999db-943">Core</span></span>

* <span data-ttu-id="999db-944">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="999db-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="999db-945">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="999db-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="999db-946">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="999db-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="999db-947">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="999db-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="999db-948">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="999db-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="999db-949">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="999db-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="999db-950">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="999db-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="999db-951">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="999db-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="999db-952">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="999db-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="999db-953">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="999db-953">core: Improved performance</span></span>
* <span data-ttu-id="999db-954">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="999db-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="999db-955">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="999db-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="999db-956">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-956">ACS</span></span>

* <span data-ttu-id="999db-957">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="999db-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="999db-958">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="999db-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="999db-959">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="999db-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="999db-960">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="999db-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-961">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-961">AppService</span></span>

* <span data-ttu-id="999db-962">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="999db-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="999db-963">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="999db-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="999db-964">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="999db-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="999db-965">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="999db-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="999db-966">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="999db-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="999db-967">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="999db-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="999db-968">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="999db-968">support slot swap with preview</span></span>
* <span data-ttu-id="999db-969">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="999db-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="999db-970">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="999db-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="999db-971">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="999db-971">CosmosDB</span></span>

* <span data-ttu-id="999db-972">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="999db-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="999db-973">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="999db-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="999db-974">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="999db-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="999db-975">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="999db-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="999db-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="999db-976">Data Lake Analytics</span></span>

* <span data-ttu-id="999db-977">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="999db-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="999db-978">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="999db-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="999db-979">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="999db-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="999db-980">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="999db-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="999db-981">Table</span><span class="sxs-lookup"><span data-stu-id="999db-981">Table</span></span>
  * <span data-ttu-id="999db-982">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="999db-982">Table valued function</span></span>
  * <span data-ttu-id="999db-983">Sicht</span><span class="sxs-lookup"><span data-stu-id="999db-983">View</span></span>
  * <span data-ttu-id="999db-984">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="999db-984">Table Statistics.</span></span> <span data-ttu-id="999db-985">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="999db-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="999db-986">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-986">Data Lake Store</span></span>

* <span data-ttu-id="999db-987">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="999db-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="999db-988">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="999db-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="999db-989">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="999db-989">missed help for access show.</span></span> <span data-ttu-id="999db-990">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="999db-990">adding it.</span></span> <span data-ttu-id="999db-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="999db-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="999db-992">Suchen</span><span class="sxs-lookup"><span data-stu-id="999db-992">Find</span></span>

* <span data-ttu-id="999db-993">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="999db-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="999db-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="999db-994">KeyVault</span></span>

* <span data-ttu-id="999db-995">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="999db-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="999db-996">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="999db-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="999db-997">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="999db-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="999db-998">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="999db-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="999db-999">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="999db-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="999db-1000">Labor</span><span class="sxs-lookup"><span data-stu-id="999db-1000">Lab</span></span>

* <span data-ttu-id="999db-1001">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="999db-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="999db-1002">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="999db-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="999db-1003">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="999db-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="999db-1004">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="999db-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="999db-1005">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="999db-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="999db-1006">Überwachen</span><span class="sxs-lookup"><span data-stu-id="999db-1006">Monitor</span></span>

* <span data-ttu-id="999db-1007">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="999db-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="999db-1008">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="999db-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="999db-1009">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-1009">Network</span></span>

* <span data-ttu-id="999db-1010">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="999db-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="999db-1011">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="999db-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="999db-1012">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="999db-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="999db-1013">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="999db-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="999db-1014">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="999db-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="999db-1015">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="999db-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="999db-1016">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="999db-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="999db-1017">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="999db-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="999db-1018">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="999db-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="999db-1019">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="999db-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="999db-1020">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="999db-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="999db-1021">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="999db-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="999db-1022">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="999db-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="999db-1023">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="999db-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="999db-1024">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="999db-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="999db-1025">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="999db-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="999db-1026">Profil</span><span class="sxs-lookup"><span data-stu-id="999db-1026">Profile</span></span>

* <span data-ttu-id="999db-1027">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="999db-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="999db-1028">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="999db-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="999db-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="999db-1029">Redis</span></span>

* <span data-ttu-id="999db-1030">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="999db-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="999db-1031">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="999db-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="999db-1032">Ressource</span><span class="sxs-lookup"><span data-stu-id="999db-1032">Resource</span></span>

* <span data-ttu-id="999db-1033">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="999db-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="999db-1034">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="999db-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="999db-1035">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="999db-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="999db-1036">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="999db-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="999db-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="999db-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="999db-1038">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="999db-1038">Add docs for az lock update.</span></span> <span data-ttu-id="999db-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="999db-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="999db-1040">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="999db-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="999db-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="999db-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="999db-1042">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="999db-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="999db-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="999db-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="999db-1044">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="999db-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="999db-1045">Rolle</span><span class="sxs-lookup"><span data-stu-id="999db-1045">Role</span></span>

* <span data-ttu-id="999db-1046">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="999db-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="999db-1047">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="999db-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="999db-1048">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="999db-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="999db-1049">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="999db-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="999db-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="999db-1050">SQL</span></span>

* <span data-ttu-id="999db-1051">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="999db-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="999db-1052">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="999db-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="999db-1053">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-1053">Storage</span></span>

* <span data-ttu-id="999db-1054">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="999db-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="999db-1055">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="999db-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="999db-1056">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="999db-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="999db-1057">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="999db-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="999db-1058">VM</span><span class="sxs-lookup"><span data-stu-id="999db-1058">VM</span></span>

* <span data-ttu-id="999db-1059">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="999db-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="999db-1060">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="999db-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="999db-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="999db-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="999db-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="999db-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="999db-1063">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="999db-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="999db-1064">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="999db-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="999db-1065">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="999db-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="999db-1066">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="999db-1066">April 3, 2017</span></span>

<span data-ttu-id="999db-1067">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="999db-1067">Version 2.0.2</span></span>

<span data-ttu-id="999db-1068">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="999db-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="999db-1069">Core</span><span class="sxs-lookup"><span data-stu-id="999db-1069">Core</span></span>

* <span data-ttu-id="999db-1070">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="999db-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="999db-1071">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="999db-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="999db-1072">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="999db-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="999db-1073">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="999db-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="999db-1074">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="999db-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="999db-1075">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="999db-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="999db-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="999db-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="999db-1077">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="999db-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="999db-1078">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="999db-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="999db-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="999db-1079">ACS</span></span>

* <span data-ttu-id="999db-1080">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="999db-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="999db-1081">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="999db-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="999db-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="999db-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="999db-1083">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="999db-1083">Add support for windows clusters.</span></span> <span data-ttu-id="999db-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="999db-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="999db-1085">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="999db-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="999db-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="999db-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="999db-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="999db-1087">AppService</span></span>

* <span data-ttu-id="999db-1088">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="999db-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="999db-1089">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="999db-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="999db-1090">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="999db-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="999db-1091">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="999db-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="999db-1092">DataLake</span><span class="sxs-lookup"><span data-stu-id="999db-1092">DataLake</span></span>

* <span data-ttu-id="999db-1093">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="999db-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="999db-1094">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="999db-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="999db-1095">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="999db-1095">DocuemntDB</span></span>

* <span data-ttu-id="999db-1096">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="999db-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="999db-1097">VM</span><span class="sxs-lookup"><span data-stu-id="999db-1097">VM</span></span>

* <span data-ttu-id="999db-1098">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="999db-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="999db-1099">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="999db-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="999db-1100">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="999db-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="999db-1101">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="999db-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="999db-1102">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="999db-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="999db-1103">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="999db-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="999db-1104">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="999db-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="999db-1105">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="999db-1105">February 27, 2017</span></span>

<span data-ttu-id="999db-1106">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="999db-1106">Version 2.0.0</span></span>

<span data-ttu-id="999db-1107">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="999db-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="999db-1108">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="999db-1108">Container Service (acs)</span></span>
- <span data-ttu-id="999db-1109">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="999db-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="999db-1110">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="999db-1110">Networking</span></span>
- <span data-ttu-id="999db-1111">Speicher</span><span class="sxs-lookup"><span data-stu-id="999db-1111">Storage</span></span>

<span data-ttu-id="999db-1112">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="999db-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="999db-1113">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="999db-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="999db-1114">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="999db-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="999db-1115">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="999db-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="999db-1116">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="999db-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="999db-1117">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="999db-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="999db-1118">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="999db-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="999db-1119">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="999db-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="999db-1120">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="999db-1120">Provide feedback from the command line with the `az feedback` command</span></span>

