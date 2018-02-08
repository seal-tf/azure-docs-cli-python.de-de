---
title: Azure CLI 2.0-Versionshinweise
description: "Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0."
keywords: Azure CLI 2.0-Versionshinweise
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/17/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 86babea3030ea932de1858a391014e5d0bba7f73
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/29/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="b580e-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="b580e-104">Azure CLI 2.0 release notes</span></span>

## <a name="january-17-2018"></a><span data-ttu-id="b580e-105">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="b580e-105">January 17, 2018</span></span>

<span data-ttu-id="b580e-106">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="b580e-106">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="b580e-107">ACR</span><span class="sxs-lookup"><span data-stu-id="b580e-107">ACR</span></span>

* <span data-ttu-id="b580e-108">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-108">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="b580e-109">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="b580e-109">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-110">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-110">ACS</span></span>

* <span data-ttu-id="b580e-111">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-111">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="b580e-112">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-112">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-113">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-113">Appservice</span></span>

* <span data-ttu-id="b580e-114">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="b580e-114">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="b580e-115">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-115">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="b580e-116">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-116">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="b580e-117">Sicherung</span><span class="sxs-lookup"><span data-stu-id="b580e-117">Backup</span></span>

* <span data-ttu-id="b580e-118">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="b580e-118">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="b580e-119">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-119">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="b580e-120">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="b580e-120">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="b580e-121">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="b580e-121">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="b580e-122">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="b580e-122">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="b580e-123">Batch</span><span class="sxs-lookup"><span data-stu-id="b580e-123">Batch</span></span>

* <span data-ttu-id="b580e-124">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="b580e-124">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="b580e-125">Cloud</span><span class="sxs-lookup"><span data-stu-id="b580e-125">Cloud</span></span>

* <span data-ttu-id="b580e-126">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="b580e-126">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="b580e-127">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b580e-127">Consumption</span></span>

* <span data-ttu-id="b580e-128">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="b580e-128">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="b580e-129">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b580e-129">Event Grid</span></span>

* <span data-ttu-id="b580e-130">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="b580e-130">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b580e-131">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="b580e-131">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b580e-132">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="b580e-132">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="b580e-133">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="b580e-133">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="b580e-134">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-134">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="b580e-135">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-135">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="b580e-136">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-136">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="b580e-137">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-137">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="b580e-138">Interactive</span><span class="sxs-lookup"><span data-stu-id="b580e-138">Interactive</span></span>

* <span data-ttu-id="b580e-139">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b580e-139">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="b580e-140">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-140">Fixed errors on startup</span></span>
* <span data-ttu-id="b580e-141">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="b580e-141">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="b580e-142">IoT</span><span class="sxs-lookup"><span data-stu-id="b580e-142">IoT</span></span>

* <span data-ttu-id="b580e-143">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-143">Added support for device provisioning service</span></span>
* <span data-ttu-id="b580e-144">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-144">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="b580e-145">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="b580e-145">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-146">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-146">Monitor</span></span>

* <span data-ttu-id="b580e-147">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-147">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="b580e-148">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b580e-148">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="b580e-149">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-149">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span> 

### <a name="network"></a><span data-ttu-id="b580e-150">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-150">Network</span></span>

* <span data-ttu-id="b580e-151">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="b580e-151">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="b580e-152">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-152">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="b580e-153">Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-153">Profile</span></span>

* <span data-ttu-id="b580e-154">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-154">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="b580e-155">Rolle</span><span class="sxs-lookup"><span data-stu-id="b580e-155">Role</span></span>

* <span data-ttu-id="b580e-156">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="b580e-156">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b580e-157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b580e-157">Service Fabric</span></span>

* <span data-ttu-id="b580e-158">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-158">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="b580e-159">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-159">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-160">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-160">VM</span></span>

* <span data-ttu-id="b580e-161">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="b580e-161">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="b580e-162">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="b580e-162">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="b580e-163">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="b580e-163">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="b580e-164">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-164">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="b580e-165">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-165">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="b580e-166">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-166">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="b580e-167">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-167">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="b580e-168">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-168">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="b580e-169">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-169">December 19, 2017</span></span>

<span data-ttu-id="b580e-170">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="b580e-170">Version 2.0.23</span></span>

* <span data-ttu-id="b580e-171">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-171">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="b580e-172">Container</span><span class="sxs-lookup"><span data-stu-id="b580e-172">Container</span></span>

* <span data-ttu-id="b580e-173">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-173">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="b580e-174">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-174">Network</span></span>

* <span data-ttu-id="b580e-175">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-175">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="b580e-176">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-176">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-177">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-177">Storage</span></span>

* <span data-ttu-id="b580e-178">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-178">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-179">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-179">VM</span></span>

* <span data-ttu-id="b580e-180">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-180">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="b580e-181">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-181">December 5, 2017</span></span>

<span data-ttu-id="b580e-182">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="b580e-182">Version 2.0.22</span></span>

* <span data-ttu-id="b580e-183">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="b580e-183">Removed `az component` commands.</span></span> <span data-ttu-id="b580e-184">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="b580e-184">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="b580e-185">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-185">Core</span></span>
* <span data-ttu-id="b580e-186">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="b580e-186">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="b580e-187">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-187">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-188">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-188">ACS</span></span>

* <span data-ttu-id="b580e-189">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-189">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="b580e-190">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="b580e-190">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="b580e-191">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="b580e-191">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="b580e-192">Advisor</span><span class="sxs-lookup"><span data-stu-id="b580e-192">Advisor</span></span>

* <span data-ttu-id="b580e-193">Erste Version</span><span class="sxs-lookup"><span data-stu-id="b580e-193">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-194">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-194">Appservice</span></span>

* <span data-ttu-id="b580e-195">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="b580e-195">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="b580e-196">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b580e-196">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="b580e-197">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-197">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="b580e-198">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b580e-198">Consumption</span></span>

* <span data-ttu-id="b580e-199">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-199">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="b580e-200">Container</span><span class="sxs-lookup"><span data-stu-id="b580e-200">Container</span></span>

* <span data-ttu-id="b580e-201">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="b580e-201">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-202">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-202">Monitor</span></span>

* <span data-ttu-id="b580e-203">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-203">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-204">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-204">Resource</span></span>

* <span data-ttu-id="b580e-205">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-205">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="b580e-206">Rolle</span><span class="sxs-lookup"><span data-stu-id="b580e-206">Role</span></span>

* <span data-ttu-id="b580e-207">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-207">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="b580e-208">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-208">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="b580e-209">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="b580e-209">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-210">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-210">SQL</span></span>

* <span data-ttu-id="b580e-211">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-211">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="b580e-212">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-212">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-213">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-213">VM</span></span>

* <span data-ttu-id="b580e-214">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-214">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="b580e-215">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-215">November 14, 2017</span></span>

<span data-ttu-id="b580e-216">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="b580e-216">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="b580e-217">ACR</span><span class="sxs-lookup"><span data-stu-id="b580e-217">ACR</span></span>

* <span data-ttu-id="b580e-218">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-218">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="b580e-219">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-219">ACS</span></span>

* <span data-ttu-id="b580e-220">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="b580e-220">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="b580e-221">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="b580e-221">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="b580e-222">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="b580e-222">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="b580e-223">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-223">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="b580e-224">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-224">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-225">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-225">Appservice</span></span>

* <span data-ttu-id="b580e-226">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-226">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="b580e-227">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-227">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="b580e-228">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-228">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="b580e-229">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-229">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="b580e-230">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-230">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="b580e-231">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="b580e-231">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="b580e-232">Batch</span><span class="sxs-lookup"><span data-stu-id="b580e-232">Batch</span></span>

* <span data-ttu-id="b580e-233">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="b580e-233">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="b580e-234">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b580e-234">Batchai</span></span>

* <span data-ttu-id="b580e-235">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-235">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="b580e-236">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-236">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="b580e-237">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-237">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="b580e-238">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-238">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="b580e-239">Cloud</span><span class="sxs-lookup"><span data-stu-id="b580e-239">Cloud</span></span>

* <span data-ttu-id="b580e-240">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="b580e-240">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="b580e-241">Container</span><span class="sxs-lookup"><span data-stu-id="b580e-241">Container</span></span>

* <span data-ttu-id="b580e-242">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-242">Added support to open multiple ports</span></span>
* <span data-ttu-id="b580e-243">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-243">Added container group restart policy</span></span>
* <span data-ttu-id="b580e-244">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-244">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="b580e-245">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b580e-245">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b580e-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b580e-246">Data Lake Analytics</span></span>

* <span data-ttu-id="b580e-247">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="b580e-247">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b580e-248">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-248">Data Lake Store</span></span>

* <span data-ttu-id="b580e-249">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="b580e-249">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="b580e-250">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b580e-250">Extension</span></span>

* <span data-ttu-id="b580e-251">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b580e-251">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="b580e-252">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b580e-252">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="b580e-253">IoT</span><span class="sxs-lookup"><span data-stu-id="b580e-253">IoT</span></span>

* <span data-ttu-id="b580e-254">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-254">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-255">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-255">Monitor</span></span>

* <span data-ttu-id="b580e-256">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-256">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="b580e-257">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-257">Network</span></span>

* <span data-ttu-id="b580e-258">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-258">Added support for CAA DNS records</span></span>
* <span data-ttu-id="b580e-259">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="b580e-259">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="b580e-260">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b580e-260">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="b580e-261">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-261">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="b580e-262">Reservations</span><span class="sxs-lookup"><span data-stu-id="b580e-262">Reservations</span></span>

* <span data-ttu-id="b580e-263">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b580e-263">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-264">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-264">Resource</span></span>

* <span data-ttu-id="b580e-265">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-265">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-266">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-266">SQL</span></span>

* <span data-ttu-id="b580e-267">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-267">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-268">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-268">Storage</span></span>

* <span data-ttu-id="b580e-269">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b580e-269">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="b580e-270">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="b580e-270">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="b580e-271">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b580e-271">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="b580e-272">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-272">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="b580e-273">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-273">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="b580e-274">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-274">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="b580e-275">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-275">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-276">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-276">VM</span></span>

* <span data-ttu-id="b580e-277">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b580e-277">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="b580e-278">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-278">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="b580e-279">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="b580e-279">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="b580e-280">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-280">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="b580e-281">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-281">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="b580e-282">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-282">October 24, 2017</span></span>

<span data-ttu-id="b580e-283">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="b580e-283">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="b580e-284">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-284">Core</span></span>

* <span data-ttu-id="b580e-285">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="b580e-285">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="b580e-286">ACR</span><span class="sxs-lookup"><span data-stu-id="b580e-286">ACR</span></span>

* <span data-ttu-id="b580e-287">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="b580e-287">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="b580e-288">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="b580e-288">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="b580e-289">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b580e-289">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-290">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-290">ACS</span></span>

* <span data-ttu-id="b580e-291">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-291">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="b580e-292">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-292">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-293">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-293">Appservice</span></span>

* <span data-ttu-id="b580e-294">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="b580e-294">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="b580e-295">Komponente</span><span class="sxs-lookup"><span data-stu-id="b580e-295">Component</span></span>

* <span data-ttu-id="b580e-296">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-296">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-297">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-297">Monitor</span></span>

* <span data-ttu-id="b580e-298">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-298">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-299">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-299">Resource</span></span>

* <span data-ttu-id="b580e-300">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-300">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="b580e-301">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="b580e-301">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-302">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-302">VM</span></span>

* <span data-ttu-id="b580e-303">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-303">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="b580e-304">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-304">October 9, 2017</span></span>

<span data-ttu-id="b580e-305">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="b580e-305">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="b580e-306">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-306">Core</span></span>

* <span data-ttu-id="b580e-307">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-307">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-308">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-308">Appservice</span></span>

* <span data-ttu-id="b580e-309">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-309">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="b580e-310">Batch</span><span class="sxs-lookup"><span data-stu-id="b580e-310">Batch</span></span>

* <span data-ttu-id="b580e-311">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="b580e-311">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="b580e-312">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b580e-312">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="b580e-313">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-313">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="b580e-314">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-314">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="b580e-315">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b580e-315">Batchai</span></span>

* <span data-ttu-id="b580e-316">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="b580e-316">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="b580e-317">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b580e-317">Keyvault</span></span>

* <span data-ttu-id="b580e-318">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="b580e-318">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="b580e-319">(#4448)</span><span class="sxs-lookup"><span data-stu-id="b580e-319">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="b580e-320">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-320">Network</span></span>

* <span data-ttu-id="b580e-321">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b580e-321">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="b580e-322">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b580e-322">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-323">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-323">Resource</span></span>

* <span data-ttu-id="b580e-324">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-324">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="b580e-325">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b580e-325">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="b580e-326">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b580e-326">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="b580e-327">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b580e-327">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-328">Sql</span><span class="sxs-lookup"><span data-stu-id="b580e-328">Sql</span></span>

* <span data-ttu-id="b580e-329">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-329">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="b580e-330">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b580e-330">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="b580e-331">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b580e-331">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-332">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-332">Storage</span></span>

* <span data-ttu-id="b580e-333">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-333">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-334">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-334">Vm</span></span>

* <span data-ttu-id="b580e-335">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="b580e-335">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="b580e-336">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-336">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="b580e-337">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-337">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="b580e-338">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-338">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="b580e-339">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-339">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="b580e-340">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-340">September 22, 2017</span></span>

<span data-ttu-id="b580e-341">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="b580e-341">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-342">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-342">Resource</span></span>

* <span data-ttu-id="b580e-343">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-343">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="b580e-344">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-344">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="b580e-345">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-345">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="b580e-346">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="b580e-346">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="b580e-347">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-347">Network</span></span>

* <span data-ttu-id="b580e-348">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-348">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="b580e-349">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-349">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="b580e-350">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-350">Added `asg` application security group commands</span></span>
* <span data-ttu-id="b580e-351">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-351">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="b580e-352">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-352">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b580e-353">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-353">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="b580e-354">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-354">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-355">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-355">Storage</span></span>

* <span data-ttu-id="b580e-356">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b580e-356">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b580e-357">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="b580e-357">Eventgrid</span></span>

* <span data-ttu-id="b580e-358">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b580e-358">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-359">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-359">SQL</span></span>

* <span data-ttu-id="b580e-360">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="b580e-360">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="b580e-361">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b580e-361">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="b580e-362">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-362">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="b580e-363">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b580e-363">Keyvault</span></span>

* <span data-ttu-id="b580e-364">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-364">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-365">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-365">VM</span></span>

* <span data-ttu-id="b580e-366">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-366">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="b580e-367">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b580e-367">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="b580e-368">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-368">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="b580e-369">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-369">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="b580e-370">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-370">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="b580e-371">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-371">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-372">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-372">ACS</span></span>

* <span data-ttu-id="b580e-373">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-373">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-374">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-374">Appservice</span></span>

* <span data-ttu-id="b580e-375">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="b580e-375">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="b580e-376">Sicherung</span><span class="sxs-lookup"><span data-stu-id="b580e-376">Backup</span></span>

* <span data-ttu-id="b580e-377">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b580e-377">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="b580e-378">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-378">September 11, 2017</span></span>

<span data-ttu-id="b580e-379">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="b580e-379">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="b580e-380">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-380">Core</span></span>

* <span data-ttu-id="b580e-381">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="b580e-381">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="b580e-382">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="b580e-382">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-383">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-383">Acs</span></span>

* <span data-ttu-id="b580e-384">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-384">Added `acs list-locations` command</span></span>
* <span data-ttu-id="b580e-385">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="b580e-385">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-386">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-386">Appservice</span></span>

* <span data-ttu-id="b580e-387">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="b580e-387">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="b580e-388">CDN</span><span class="sxs-lookup"><span data-stu-id="b580e-388">CDN</span></span>

* <span data-ttu-id="b580e-389">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b580e-389">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="b580e-390">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b580e-390">Extension</span></span>

* <span data-ttu-id="b580e-391">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="b580e-391">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="b580e-392">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b580e-392">Keyvault</span></span>

* <span data-ttu-id="b580e-393">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="b580e-393">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="b580e-394">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-394">Network</span></span>

* <span data-ttu-id="b580e-395">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-395">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b580e-396">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b580e-396">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="b580e-397">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-397">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="b580e-398">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-398">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b580e-399">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-399">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-400">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-400">Resource</span></span>

* <span data-ttu-id="b580e-401">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="b580e-401">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="b580e-402">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="b580e-402">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="b580e-403">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="b580e-403">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="b580e-404">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="b580e-404">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-405">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-405">SQL</span></span>

* <span data-ttu-id="b580e-406">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-406">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-407">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-407">VM</span></span>

* <span data-ttu-id="b580e-408">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="b580e-408">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="b580e-409">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="b580e-409">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="b580e-410">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-410">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="b580e-411">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="b580e-411">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="b580e-412">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="b580e-412">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="b580e-413">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-413">August 31, 2017</span></span>

<span data-ttu-id="b580e-414">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="b580e-414">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="b580e-415">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b580e-415">Keyvault</span></span>

* <span data-ttu-id="b580e-416">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="b580e-416">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="b580e-417">Sf</span><span class="sxs-lookup"><span data-stu-id="b580e-417">Sf</span></span>

* <span data-ttu-id="b580e-418">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b580e-418">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-419">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-419">Storage</span></span>

* <span data-ttu-id="b580e-420">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="b580e-420">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="b580e-421">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="b580e-421">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="b580e-422">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-422">August 28, 2017</span></span>

<span data-ttu-id="b580e-423">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="b580e-423">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="b580e-424">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="b580e-424">CLI</span></span>

* <span data-ttu-id="b580e-425">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-425">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-426">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-426">ACS</span></span>

* <span data-ttu-id="b580e-427">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="b580e-427">Corrected preview regions.</span></span>
* <span data-ttu-id="b580e-428">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="b580e-428">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="b580e-429">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="b580e-429">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-430">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-430">Appservice</span></span>

* <span data-ttu-id="b580e-431">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-431">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="b580e-432">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-432">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="b580e-433">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b580e-433">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="b580e-434">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="b580e-434">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="b580e-435">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="b580e-435">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="b580e-436">IoT</span><span class="sxs-lookup"><span data-stu-id="b580e-436">IoT</span></span>

* <span data-ttu-id="b580e-437">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="b580e-437">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="b580e-438">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-438">Network</span></span>

* <span data-ttu-id="b580e-439">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-439">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b580e-440">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-440">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="b580e-441">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-441">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b580e-442">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-442">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b580e-443">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-443">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="b580e-444">Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-444">Profile</span></span>

* <span data-ttu-id="b580e-445">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b580e-445">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b580e-446">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b580e-446">Service Fabric</span></span>

* <span data-ttu-id="b580e-447">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b580e-447">Preview release</span></span>
* <span data-ttu-id="b580e-448">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="b580e-448">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="b580e-449">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-449">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="b580e-450">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-450">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-451">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-451">Storage</span></span>

* <span data-ttu-id="b580e-452">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b580e-452">Enabled setting blob tier</span></span>
* <span data-ttu-id="b580e-453">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-453">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="b580e-454">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-454">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="b580e-455">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b580e-455">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="b580e-456">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-456">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="b580e-457">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="b580e-457">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-458">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-458">VM</span></span>

* <span data-ttu-id="b580e-459">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-459">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="b580e-460">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b580e-460">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="b580e-461">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-461">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="b580e-462">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="b580e-462">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="b580e-463">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-463">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="b580e-464">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b580e-464">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="b580e-465">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-465">August 15, 2017</span></span>

<span data-ttu-id="b580e-466">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="b580e-466">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-467">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-467">ACS</span></span>

* <span data-ttu-id="b580e-468">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-468">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-469">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-469">Appservice</span></span>

* <span data-ttu-id="b580e-470">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-470">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="b580e-471">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b580e-471">Event Grid</span></span>

* <span data-ttu-id="b580e-472">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-472">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="b580e-473">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-473">August 11, 2017</span></span>

<span data-ttu-id="b580e-474">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="b580e-474">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-475">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-475">ACS</span></span>

* <span data-ttu-id="b580e-476">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-476">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="b580e-477">Batch</span><span class="sxs-lookup"><span data-stu-id="b580e-477">Batch</span></span>

* <span data-ttu-id="b580e-478">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b580e-478">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="b580e-479">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-479">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="b580e-480">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-480">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="b580e-481">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="b580e-481">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="b580e-482">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="b580e-482">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="b580e-483">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-483">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="b580e-484">Komponente</span><span class="sxs-lookup"><span data-stu-id="b580e-484">Component</span></span>

* <span data-ttu-id="b580e-485">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-485">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="b580e-486">Container</span><span class="sxs-lookup"><span data-stu-id="b580e-486">Container</span></span>

* <span data-ttu-id="b580e-487">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="b580e-487">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="b580e-488">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-488">Data Lake Store</span></span>

* <span data-ttu-id="b580e-489">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b580e-489">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="b580e-490">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b580e-490">Event Grid</span></span>

* <span data-ttu-id="b580e-491">Erste Version</span><span class="sxs-lookup"><span data-stu-id="b580e-491">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="b580e-492">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-492">Network</span></span>

* <span data-ttu-id="b580e-493">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-493">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="b580e-494">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="b580e-494">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="b580e-495">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="b580e-495">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="b580e-496">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="b580e-496">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="b580e-497">Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-497">Profile</span></span>

* <span data-ttu-id="b580e-498">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="b580e-498">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-499">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-499">Storage</span></span>

* <span data-ttu-id="b580e-500">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b580e-500">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-501">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-501">VM</span></span>

* <span data-ttu-id="b580e-502">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b580e-502">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="b580e-503">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b580e-503">Exposed `list-skus` command</span></span>
* <span data-ttu-id="b580e-504">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="b580e-504">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="b580e-505">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="b580e-505">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="b580e-506">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-506">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="b580e-507">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-507">July 28, 2017</span></span>

<span data-ttu-id="b580e-508">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="b580e-508">Version 2.0.12</span></span>

* <span data-ttu-id="b580e-509">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-509">Added container commands</span></span>
* <span data-ttu-id="b580e-510">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-510">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="b580e-511">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-511">Core</span></span>

* <span data-ttu-id="b580e-512">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="b580e-512">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="b580e-513">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-513">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="b580e-514">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="b580e-514">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="b580e-515">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="b580e-515">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="b580e-516">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="b580e-516">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="b580e-517">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="b580e-517">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="b580e-518">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="b580e-518">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b580e-519">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="b580e-519">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="b580e-520">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="b580e-520">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="b580e-521">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-521">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="b580e-522">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="b580e-522">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="b580e-523">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="b580e-523">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="b580e-524">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="b580e-524">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="b580e-525">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="b580e-525">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="b580e-526">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="b580e-526">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="b580e-527">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="b580e-527">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="b580e-528">ACR</span><span class="sxs-lookup"><span data-stu-id="b580e-528">ACR</span></span>

* <span data-ttu-id="b580e-529">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-529">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="b580e-530">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="b580e-530">Support SKU update for managed registries</span></span>
* <span data-ttu-id="b580e-531">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-531">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="b580e-532">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-532">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="b580e-533">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-533">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="b580e-534">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-534">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-535">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-535">ACS</span></span>

* <span data-ttu-id="b580e-536">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="b580e-536">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-537">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-537">Appservice</span></span>

* <span data-ttu-id="b580e-538">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="b580e-538">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="b580e-539">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="b580e-539">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="b580e-540">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="b580e-540">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="b580e-541">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="b580e-541">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="b580e-542">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="b580e-542">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="b580e-543">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="b580e-543">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="b580e-544">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="b580e-544">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="b580e-545">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="b580e-545">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="b580e-546">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="b580e-546">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="b580e-547">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="b580e-547">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="b580e-548">Batch</span><span class="sxs-lookup"><span data-stu-id="b580e-548">Batch</span></span>

* <span data-ttu-id="b580e-549">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b580e-549">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="b580e-550">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-550">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="b580e-551">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-551">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="b580e-552">CDN</span><span class="sxs-lookup"><span data-stu-id="b580e-552">CDN</span></span>

* <span data-ttu-id="b580e-553">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="b580e-553">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="b580e-554">Cloud</span><span class="sxs-lookup"><span data-stu-id="b580e-554">Cloud</span></span>

* <span data-ttu-id="b580e-555">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="b580e-555">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="b580e-556">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="b580e-556">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="b580e-557">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="b580e-557">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="b580e-558">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="b580e-558">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="b580e-559">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b580e-559">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b580e-560">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b580e-560">CosmosDB</span></span>

* <span data-ttu-id="b580e-561">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="b580e-561">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="b580e-562">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-562">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b580e-563">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b580e-563">Data Lake Analytics</span></span>

* <span data-ttu-id="b580e-564">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-564">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="b580e-565">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-565">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="b580e-566">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-566">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b580e-567">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-567">Data Lake Store</span></span>

* <span data-ttu-id="b580e-568">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-568">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="b580e-569">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="b580e-569">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="b580e-570">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b580e-570">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="b580e-571">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b580e-571">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="b580e-572">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="b580e-572">Interactive</span></span>

* <span data-ttu-id="b580e-573">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-573">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="b580e-574">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-574">Increased test coverage</span></span>
* <span data-ttu-id="b580e-575">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="b580e-575">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="b580e-576">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="b580e-576">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="b580e-577">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="b580e-577">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="b580e-578">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="b580e-578">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="b580e-579">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="b580e-579">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b580e-580">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-580">Added `--progress` flag</span></span>
* <span data-ttu-id="b580e-581">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-581">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="b580e-582">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="b580e-582">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="b580e-583">IoT</span><span class="sxs-lookup"><span data-stu-id="b580e-583">IoT</span></span>

* <span data-ttu-id="b580e-584">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="b580e-584">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="b580e-585">(3934)</span><span class="sxs-lookup"><span data-stu-id="b580e-585">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="b580e-586">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="b580e-586">Key vault</span></span>

* <span data-ttu-id="b580e-587">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b580e-587">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="b580e-588">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b580e-588">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="b580e-589">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b580e-589">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b580e-590">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b580e-590">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b580e-591">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b580e-591">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="b580e-592">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="b580e-592">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="b580e-593">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b580e-593">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="b580e-594">(3307)</span><span class="sxs-lookup"><span data-stu-id="b580e-594">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="b580e-595">Labor</span><span class="sxs-lookup"><span data-stu-id="b580e-595">Lab</span></span>

* <span data-ttu-id="b580e-596">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-596">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="b580e-597">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-597">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-598">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-598">Monitor</span></span>

* <span data-ttu-id="b580e-599">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="b580e-599">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="b580e-600">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-600">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="b580e-601">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-601">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="b580e-602">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-602">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="b580e-603">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b580e-603">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="b580e-604">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="b580e-604">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="b580e-605">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="b580e-605">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="b580e-606">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="b580e-606">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="b580e-607">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="b580e-607">`location` no longer required</span></span>
  * <span data-ttu-id="b580e-608">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="b580e-608">Add name and ID support for target</span></span>
  * <span data-ttu-id="b580e-609">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="b580e-609">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="b580e-610">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="b580e-610">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="b580e-611">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b580e-611">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="b580e-612">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="b580e-612">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="b580e-613">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="b580e-613">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="b580e-614">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-614">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="b580e-615">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-615">Network</span></span>

* <span data-ttu-id="b580e-616">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-616">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="b580e-617">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-617">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="b580e-618">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b580e-618">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="b580e-619">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b580e-619">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="b580e-620">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="b580e-620">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="b580e-621">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-621">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="b580e-622">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="b580e-622">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="b580e-623">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="b580e-623">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="b580e-624">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="b580e-624">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="b580e-625">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b580e-625">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="b580e-626">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-626">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="b580e-627">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-627">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="b580e-628">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="b580e-628">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="b580e-629">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-629">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="b580e-630">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-630">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="b580e-631">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-631">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="b580e-632">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-632">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="b580e-633">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="b580e-633">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="b580e-634">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-634">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="b580e-635">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-635">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="b580e-636">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="b580e-636">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="b580e-637">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b580e-637">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="b580e-638">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-638">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="b580e-639">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b580e-639">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="b580e-640">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b580e-640">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="b580e-641">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b580e-641">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="b580e-642">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b580e-642">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="b580e-643">Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-643">Profile</span></span>

* <span data-ttu-id="b580e-644">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="b580e-644">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="b580e-645">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="b580e-645">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="b580e-646">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="b580e-646">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="b580e-647">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-647">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="b580e-648">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="b580e-648">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="b580e-649">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b580e-649">RDBMS</span></span>

* <span data-ttu-id="b580e-650">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="b580e-650">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="b580e-651">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="b580e-651">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="b580e-652">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="b580e-652">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="b580e-653">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="b580e-653">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-654">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-654">Resource</span></span>

* <span data-ttu-id="b580e-655">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-655">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="b580e-656">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="b580e-656">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="b580e-657">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-657">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="b580e-658">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="b580e-658">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="b580e-659">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="b580e-659">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="b580e-660">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="b580e-660">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="b580e-661">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="b580e-661">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="b580e-662">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-662">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="b580e-663">Rolle</span><span class="sxs-lookup"><span data-stu-id="b580e-663">Role</span></span>

* <span data-ttu-id="b580e-664">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="b580e-664">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="b580e-665">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="b580e-665">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="b580e-666">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="b580e-666">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="b580e-667">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="b580e-667">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="b580e-668">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-668">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b580e-669">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b580e-669">Service Fabric</span></span>
* <span data-ttu-id="b580e-670">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="b580e-670">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="b580e-671">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="b580e-671">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="b580e-672">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="b580e-672">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-673">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-673">SQL</span></span>

* <span data-ttu-id="b580e-674">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-674">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="b580e-675">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="b580e-675">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="b580e-676">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-676">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-677">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-677">Storage</span></span>

* <span data-ttu-id="b580e-678">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="b580e-678">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="b580e-679">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b580e-679">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="b580e-680">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="b580e-680">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="b580e-681">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="b580e-681">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="b580e-682">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="b580e-682">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="b580e-683">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="b580e-683">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-684">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-684">VM</span></span>

* <span data-ttu-id="b580e-685">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="b580e-685">Support configuring nsg</span></span>
* <span data-ttu-id="b580e-686">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="b580e-686">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="b580e-687">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="b580e-687">Support managed service identities</span></span>
* <span data-ttu-id="b580e-688">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="b580e-688">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="b580e-689">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="b580e-689">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="b580e-690">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-690">May 10, 2017</span></span>

<span data-ttu-id="b580e-691">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="b580e-691">Version 2.0.6</span></span>

* <span data-ttu-id="b580e-692">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="b580e-692">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="b580e-693">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="b580e-693">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="b580e-694">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="b580e-694">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="b580e-695">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="b580e-695">Include Cognitive Services module.</span></span>
* <span data-ttu-id="b580e-696">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="b580e-696">Include Service Fabric module.</span></span>
* <span data-ttu-id="b580e-697">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="b580e-697">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="b580e-698">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="b580e-698">Add support for CDN commands.</span></span>
* <span data-ttu-id="b580e-699">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="b580e-699">Remove Container module.</span></span>
* <span data-ttu-id="b580e-700">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="b580e-700">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="b580e-701">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b580e-701">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="b580e-702">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-702">Core</span></span>

* <span data-ttu-id="b580e-703">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="b580e-703">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="b580e-704">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="b580e-704">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="b580e-705">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="b580e-705">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="b580e-706">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="b580e-706">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="b580e-707">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="b580e-707">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="b580e-708">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="b580e-708">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="b580e-709">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="b580e-709">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="b580e-710">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="b580e-710">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="b580e-711">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="b580e-711">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="b580e-712">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="b580e-712">core: Improved performance</span></span>
* <span data-ttu-id="b580e-713">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="b580e-713">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="b580e-714">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="b580e-714">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-715">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-715">ACS</span></span>

* <span data-ttu-id="b580e-716">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b580e-716">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="b580e-717">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="b580e-717">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="b580e-718">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="b580e-718">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="b580e-719">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="b580e-719">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-720">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-720">AppService</span></span>

* <span data-ttu-id="b580e-721">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="b580e-721">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="b580e-722">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="b580e-722">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="b580e-723">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="b580e-723">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="b580e-724">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="b580e-724">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="b580e-725">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="b580e-725">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="b580e-726">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="b580e-726">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="b580e-727">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="b580e-727">support slot swap with preview</span></span>
* <span data-ttu-id="b580e-728">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="b580e-728">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="b580e-729">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="b580e-729">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b580e-730">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b580e-730">CosmosDB</span></span>

* <span data-ttu-id="b580e-731">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="b580e-731">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="b580e-732">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="b580e-732">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="b580e-733">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="b580e-733">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="b580e-734">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="b580e-734">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b580e-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b580e-735">Data Lake Analytics</span></span>

* <span data-ttu-id="b580e-736">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="b580e-736">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="b580e-737">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="b580e-737">Add support for new catalog item type: package.</span></span> <span data-ttu-id="b580e-738">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="b580e-738">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="b580e-739">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="b580e-739">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="b580e-740">Table</span><span class="sxs-lookup"><span data-stu-id="b580e-740">Table</span></span>
  * <span data-ttu-id="b580e-741">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="b580e-741">Table valued function</span></span>
  * <span data-ttu-id="b580e-742">Sicht</span><span class="sxs-lookup"><span data-stu-id="b580e-742">View</span></span>
  * <span data-ttu-id="b580e-743">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="b580e-743">Table Statistics.</span></span> <span data-ttu-id="b580e-744">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="b580e-744">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b580e-745">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-745">Data Lake Store</span></span>

* <span data-ttu-id="b580e-746">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="b580e-746">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="b580e-747">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b580e-747">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="b580e-748">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="b580e-748">missed help for access show.</span></span> <span data-ttu-id="b580e-749">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b580e-749">adding it.</span></span> <span data-ttu-id="b580e-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="b580e-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="b580e-751">Suchen</span><span class="sxs-lookup"><span data-stu-id="b580e-751">Find</span></span>

* <span data-ttu-id="b580e-752">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="b580e-752">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="b580e-753">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b580e-753">KeyVault</span></span>

* <span data-ttu-id="b580e-754">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="b580e-754">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="b580e-755">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="b580e-755">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="b580e-756">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="b580e-756">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="b580e-757">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="b580e-757">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="b580e-758">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="b580e-758">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="b580e-759">Labor</span><span class="sxs-lookup"><span data-stu-id="b580e-759">Lab</span></span>

* <span data-ttu-id="b580e-760">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="b580e-760">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="b580e-761">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="b580e-761">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="b580e-762">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="b580e-762">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="b580e-763">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="b580e-763">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="b580e-764">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="b580e-764">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="b580e-765">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b580e-765">Monitor</span></span>

* <span data-ttu-id="b580e-766">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="b580e-766">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="b580e-767">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="b580e-767">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="b580e-768">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-768">Network</span></span>

* <span data-ttu-id="b580e-769">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="b580e-769">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="b580e-770">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="b580e-770">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="b580e-771">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="b580e-771">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="b580e-772">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="b580e-772">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="b580e-773">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="b580e-773">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="b580e-774">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="b580e-774">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="b580e-775">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="b580e-775">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="b580e-776">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="b580e-776">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="b580e-777">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="b580e-777">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="b580e-778">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="b580e-778">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="b580e-779">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="b580e-779">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="b580e-780">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="b580e-780">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="b580e-781">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="b580e-781">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="b580e-782">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="b580e-782">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="b580e-783">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b580e-783">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="b580e-784">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="b580e-784">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="b580e-785">Profil</span><span class="sxs-lookup"><span data-stu-id="b580e-785">Profile</span></span>

* <span data-ttu-id="b580e-786">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="b580e-786">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="b580e-787">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="b580e-787">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="b580e-788">Redis</span><span class="sxs-lookup"><span data-stu-id="b580e-788">Redis</span></span>

* <span data-ttu-id="b580e-789">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="b580e-789">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="b580e-790">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="b580e-790">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="b580e-791">Ressource</span><span class="sxs-lookup"><span data-stu-id="b580e-791">Resource</span></span>

* <span data-ttu-id="b580e-792">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="b580e-792">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="b580e-793">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="b580e-793">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="b580e-794">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="b580e-794">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="b580e-795">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="b580e-795">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="b580e-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="b580e-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="b580e-797">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="b580e-797">Add docs for az lock update.</span></span> <span data-ttu-id="b580e-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="b580e-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="b580e-799">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="b580e-799">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="b580e-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="b580e-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="b580e-801">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="b580e-801">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="b580e-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="b580e-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="b580e-803">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="b580e-803">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="b580e-804">Rolle</span><span class="sxs-lookup"><span data-stu-id="b580e-804">Role</span></span>

* <span data-ttu-id="b580e-805">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="b580e-805">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="b580e-806">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="b580e-806">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="b580e-807">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="b580e-807">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="b580e-808">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="b580e-808">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="b580e-809">SQL</span><span class="sxs-lookup"><span data-stu-id="b580e-809">SQL</span></span>

* <span data-ttu-id="b580e-810">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="b580e-810">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="b580e-811">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="b580e-811">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="b580e-812">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-812">Storage</span></span>

* <span data-ttu-id="b580e-813">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="b580e-813">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="b580e-814">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="b580e-814">Add support for incremental blob copy</span></span>
* <span data-ttu-id="b580e-815">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="b580e-815">Add support for large block blob upload</span></span>
* <span data-ttu-id="b580e-816">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="b580e-816">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-817">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-817">VM</span></span>

* <span data-ttu-id="b580e-818">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="b580e-818">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="b580e-819">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="b580e-819">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="b580e-820">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="b580e-820">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="b580e-821">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="b580e-821">az vm/vmss disk</span></span>
  3. <span data-ttu-id="b580e-822">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="b580e-822">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="b580e-823">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="b580e-823">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="b580e-824">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="b580e-824">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="b580e-825">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-825">April 3, 2017</span></span>

<span data-ttu-id="b580e-826">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="b580e-826">Version 2.0.2</span></span>

<span data-ttu-id="b580e-827">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="b580e-827">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="b580e-828">Core</span><span class="sxs-lookup"><span data-stu-id="b580e-828">Core</span></span>

* <span data-ttu-id="b580e-829">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="b580e-829">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="b580e-830">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="b580e-830">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="b580e-831">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="b580e-831">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="b580e-832">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b580e-832">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b580e-833">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="b580e-833">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="b580e-834">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="b580e-834">Add prompting for missing template parameters.</span></span> <span data-ttu-id="b580e-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="b580e-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="b580e-836">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="b580e-836">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="b580e-837">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="b580e-837">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="b580e-838">ACS</span><span class="sxs-lookup"><span data-stu-id="b580e-838">ACS</span></span>

* <span data-ttu-id="b580e-839">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="b580e-839">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="b580e-840">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="b580e-840">Add support for ssh key password prompting.</span></span> <span data-ttu-id="b580e-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="b580e-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="b580e-842">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="b580e-842">Add support for windows clusters.</span></span> <span data-ttu-id="b580e-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="b580e-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="b580e-844">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="b580e-844">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="b580e-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="b580e-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="b580e-846">AppService</span><span class="sxs-lookup"><span data-stu-id="b580e-846">AppService</span></span>

* <span data-ttu-id="b580e-847">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="b580e-847">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="b580e-848">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="b580e-848">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="b580e-849">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="b580e-849">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="b580e-850">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="b580e-850">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="b580e-851">DataLake</span><span class="sxs-lookup"><span data-stu-id="b580e-851">DataLake</span></span>

* <span data-ttu-id="b580e-852">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="b580e-852">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="b580e-853">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="b580e-853">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="b580e-854">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="b580e-854">DocuemntDB</span></span>

* <span data-ttu-id="b580e-855">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="b580e-855">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="b580e-856">VM</span><span class="sxs-lookup"><span data-stu-id="b580e-856">VM</span></span>

* <span data-ttu-id="b580e-857">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="b580e-857">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="b580e-858">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="b580e-858">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="b580e-859">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="b580e-859">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="b580e-860">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b580e-860">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b580e-861">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="b580e-861">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="b580e-862">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="b580e-862">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="b580e-863">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="b580e-863">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="b580e-864">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="b580e-864">February 27, 2017</span></span>

<span data-ttu-id="b580e-865">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="b580e-865">Version 2.0.0</span></span>

<span data-ttu-id="b580e-866">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="b580e-866">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="b580e-867">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="b580e-867">General availability applies to these command modules:</span></span>
- <span data-ttu-id="b580e-868">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="b580e-868">Container Service (acs)</span></span>
- <span data-ttu-id="b580e-869">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="b580e-869">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="b580e-870">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b580e-870">Networking</span></span>
- <span data-ttu-id="b580e-871">Speicher</span><span class="sxs-lookup"><span data-stu-id="b580e-871">Storage</span></span>

<span data-ttu-id="b580e-872">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b580e-872">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="b580e-873">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="b580e-873">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="b580e-874">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="b580e-874">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="b580e-875">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="b580e-875">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="b580e-876">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="b580e-876">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="b580e-877">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="b580e-877">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="b580e-878">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="b580e-878">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="b580e-879">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="b580e-879">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="b580e-880">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="b580e-880">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="b580e-881">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="b580e-881">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="b580e-882">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="b580e-882">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="b580e-883">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="b580e-883">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="b580e-884">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="b580e-884">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="b580e-885">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="b580e-885">Provide feedback from the command line with the `az feedback` command.</span></span>

