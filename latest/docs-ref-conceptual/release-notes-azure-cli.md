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
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="fa726-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="fa726-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-22-2017"></a><span data-ttu-id="fa726-105">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-105">September 22, 2017</span></span>

<span data-ttu-id="fa726-106">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="fa726-106">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="fa726-107">Ressource</span><span class="sxs-lookup"><span data-stu-id="fa726-107">Resource</span></span>

* <span data-ttu-id="fa726-108">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-108">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="fa726-109">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-109">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="fa726-110">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-110">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="fa726-111">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="fa726-111">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="fa726-112">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-112">Network</span></span>

* <span data-ttu-id="fa726-113">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-113">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="fa726-114">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-114">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="fa726-115">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-115">Added `asg` application security group commands</span></span>
* <span data-ttu-id="fa726-116">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-116">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="fa726-117">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-117">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fa726-118">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-118">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="fa726-119">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-119">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-120">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-120">Storage</span></span>

* <span data-ttu-id="fa726-121">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fa726-121">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fa726-122">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="fa726-122">Eventgrid</span></span>

* <span data-ttu-id="fa726-123">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fa726-123">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="fa726-124">SQL</span><span class="sxs-lookup"><span data-stu-id="fa726-124">SQL</span></span>

* <span data-ttu-id="fa726-125">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="fa726-125">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="fa726-126">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa726-126">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="fa726-127">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-127">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="fa726-128">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa726-128">Keyvault</span></span>

* <span data-ttu-id="fa726-129">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-129">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-130">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-130">VM</span></span>

* <span data-ttu-id="fa726-131">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-131">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="fa726-132">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fa726-132">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="fa726-133">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-133">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="fa726-134">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-134">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="fa726-135">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-135">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="fa726-136">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-136">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-137">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-137">ACS</span></span>

* <span data-ttu-id="fa726-138">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-138">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-139">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-139">Appservice</span></span>

* <span data-ttu-id="fa726-140">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="fa726-140">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fa726-141">Backup </span><span class="sxs-lookup"><span data-stu-id="fa726-141">Backup</span></span>

* <span data-ttu-id="fa726-142">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fa726-142">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="fa726-143">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-143">September 11, 2017</span></span>

<span data-ttu-id="fa726-144">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="fa726-144">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="fa726-145">Core</span><span class="sxs-lookup"><span data-stu-id="fa726-145">Core</span></span>

* <span data-ttu-id="fa726-146">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="fa726-146">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="fa726-147">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="fa726-147">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-148">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-148">Acs</span></span>

* <span data-ttu-id="fa726-149">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-149">Added `acs list-locations` command</span></span>
* <span data-ttu-id="fa726-150">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="fa726-150">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-151">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-151">Appservice</span></span>

* <span data-ttu-id="fa726-152">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="fa726-152">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="fa726-153">CDN</span><span class="sxs-lookup"><span data-stu-id="fa726-153">CDN</span></span>

* <span data-ttu-id="fa726-154">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fa726-154">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="fa726-155">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fa726-155">Extension</span></span>

* <span data-ttu-id="fa726-156">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="fa726-156">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="fa726-157">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa726-157">Keyvault</span></span>

* <span data-ttu-id="fa726-158">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="fa726-158">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="fa726-159">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-159">Network</span></span>

* <span data-ttu-id="fa726-160">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-160">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fa726-161">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fa726-161">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="fa726-162">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-162">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="fa726-163">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-163">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fa726-164">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-164">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="fa726-165">Ressource</span><span class="sxs-lookup"><span data-stu-id="fa726-165">Resource</span></span>

* <span data-ttu-id="fa726-166">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="fa726-166">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="fa726-167">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="fa726-167">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="fa726-168">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="fa726-168">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="fa726-169">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="fa726-169">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="fa726-170">SQL</span><span class="sxs-lookup"><span data-stu-id="fa726-170">SQL</span></span>

* <span data-ttu-id="fa726-171">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-171">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-172">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-172">VM</span></span>

* <span data-ttu-id="fa726-173">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="fa726-173">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="fa726-174">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="fa726-174">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="fa726-175">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-175">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="fa726-176">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="fa726-176">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="fa726-177">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="fa726-177">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="fa726-178">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-178">August 31, 2017</span></span>

<span data-ttu-id="fa726-179">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="fa726-179">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="fa726-180">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa726-180">Keyvault</span></span>

* <span data-ttu-id="fa726-181">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="fa726-181">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="fa726-182">Sf</span><span class="sxs-lookup"><span data-stu-id="fa726-182">Sf</span></span>

* <span data-ttu-id="fa726-183">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="fa726-183">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-184">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-184">Storage</span></span>

* <span data-ttu-id="fa726-185">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="fa726-185">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="fa726-186">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="fa726-186">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="fa726-187">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-187">August 28, 2017</span></span>

<span data-ttu-id="fa726-188">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="fa726-188">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="fa726-189">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="fa726-189">CLI</span></span>

* <span data-ttu-id="fa726-190">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fa726-190">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-191">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-191">ACS</span></span>

* <span data-ttu-id="fa726-192">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="fa726-192">Corrected preview regions.</span></span>
* <span data-ttu-id="fa726-193">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="fa726-193">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="fa726-194">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="fa726-194">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-195">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-195">Appservice</span></span>

* <span data-ttu-id="fa726-196">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-196">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="fa726-197">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-197">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="fa726-198">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fa726-198">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="fa726-199">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="fa726-199">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="fa726-200">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="fa726-200">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="fa726-201">IoT</span><span class="sxs-lookup"><span data-stu-id="fa726-201">IoT</span></span>

* <span data-ttu-id="fa726-202">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="fa726-202">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="fa726-203">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-203">Network</span></span>

* <span data-ttu-id="fa726-204">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-204">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fa726-205">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-205">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="fa726-206">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-206">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fa726-207">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-207">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fa726-208">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-208">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="fa726-209">Profil</span><span class="sxs-lookup"><span data-stu-id="fa726-209">Profile</span></span>

* <span data-ttu-id="fa726-210">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fa726-210">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fa726-211">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fa726-211">Service Fabric</span></span>

* <span data-ttu-id="fa726-212">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fa726-212">Preview release</span></span>
* <span data-ttu-id="fa726-213">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="fa726-213">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="fa726-214">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-214">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="fa726-215">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-215">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-216">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-216">Storage</span></span>

* <span data-ttu-id="fa726-217">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fa726-217">Enabled setting blob tier</span></span>
* <span data-ttu-id="fa726-218">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-218">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="fa726-219">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-219">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="fa726-220">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fa726-220">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="fa726-221">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-221">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="fa726-222">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="fa726-222">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-223">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-223">VM</span></span>

* <span data-ttu-id="fa726-224">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="fa726-224">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="fa726-225">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fa726-225">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="fa726-226">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-226">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="fa726-227">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="fa726-227">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="fa726-228">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-228">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="fa726-229">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fa726-229">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="fa726-230">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-230">August 15, 2017</span></span>

<span data-ttu-id="fa726-231">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="fa726-231">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-232">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-232">ACS</span></span>

* <span data-ttu-id="fa726-233">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="fa726-233">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-234">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-234">Appservice</span></span>

* <span data-ttu-id="fa726-235">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-235">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="fa726-236">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fa726-236">Event Grid</span></span>

* <span data-ttu-id="fa726-237">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-237">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="fa726-238">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-238">August 11, 2017</span></span>

<span data-ttu-id="fa726-239">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="fa726-239">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-240">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-240">ACS</span></span>

* <span data-ttu-id="fa726-241">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-241">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="fa726-242">Batch</span><span class="sxs-lookup"><span data-stu-id="fa726-242">Batch</span></span>

* <span data-ttu-id="fa726-243">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fa726-243">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="fa726-244">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-244">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="fa726-245">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-245">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="fa726-246">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="fa726-246">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="fa726-247">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="fa726-247">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="fa726-248">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-248">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="fa726-249">Komponente</span><span class="sxs-lookup"><span data-stu-id="fa726-249">Component</span></span>

* <span data-ttu-id="fa726-250">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-250">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="fa726-251">Container</span><span class="sxs-lookup"><span data-stu-id="fa726-251">Container</span></span>

* <span data-ttu-id="fa726-252">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="fa726-252">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="fa726-253">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-253">Data Lake Store</span></span>

* <span data-ttu-id="fa726-254">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fa726-254">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="fa726-255">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fa726-255">Event Grid</span></span>

* <span data-ttu-id="fa726-256">Erste Version</span><span class="sxs-lookup"><span data-stu-id="fa726-256">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="fa726-257">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-257">Network</span></span>

* <span data-ttu-id="fa726-258">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="fa726-258">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="fa726-259">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="fa726-259">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="fa726-260">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="fa726-260">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="fa726-261">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="fa726-261">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="fa726-262">Profil</span><span class="sxs-lookup"><span data-stu-id="fa726-262">Profile</span></span>

* <span data-ttu-id="fa726-263">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="fa726-263">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-264">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-264">Storage</span></span>

* <span data-ttu-id="fa726-265">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fa726-265">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-266">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-266">VM</span></span>

* <span data-ttu-id="fa726-267">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fa726-267">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="fa726-268">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fa726-268">Exposed `list-skus` command</span></span>
* <span data-ttu-id="fa726-269">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="fa726-269">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="fa726-270">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="fa726-270">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="fa726-271">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-271">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="fa726-272">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-272">July 28, 2017</span></span>

<span data-ttu-id="fa726-273">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="fa726-273">Version 2.0.12</span></span>

* <span data-ttu-id="fa726-274">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-274">Added container commands</span></span>
* <span data-ttu-id="fa726-275">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-275">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="fa726-276">Core</span><span class="sxs-lookup"><span data-stu-id="fa726-276">Core</span></span>

* <span data-ttu-id="fa726-277">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="fa726-277">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="fa726-278">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-278">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="fa726-279">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="fa726-279">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="fa726-280">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="fa726-280">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="fa726-281">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="fa726-281">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="fa726-282">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="fa726-282">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="fa726-283">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="fa726-283">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fa726-284">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="fa726-284">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="fa726-285">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="fa726-285">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="fa726-286">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="fa726-286">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="fa726-287">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="fa726-287">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="fa726-288">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="fa726-288">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="fa726-289">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="fa726-289">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="fa726-290">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="fa726-290">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="fa726-291">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="fa726-291">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="fa726-292">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="fa726-292">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="fa726-293">ACR</span><span class="sxs-lookup"><span data-stu-id="fa726-293">ACR</span></span>

* <span data-ttu-id="fa726-294">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-294">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="fa726-295">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="fa726-295">Support SKU update for managed registries</span></span>
* <span data-ttu-id="fa726-296">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-296">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="fa726-297">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-297">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="fa726-298">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-298">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="fa726-299">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-299">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-300">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-300">ACS</span></span>

* <span data-ttu-id="fa726-301">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="fa726-301">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-302">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-302">Appservice</span></span>

* <span data-ttu-id="fa726-303">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="fa726-303">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="fa726-304">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="fa726-304">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="fa726-305">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="fa726-305">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="fa726-306">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="fa726-306">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="fa726-307">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="fa726-307">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="fa726-308">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="fa726-308">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="fa726-309">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="fa726-309">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="fa726-310">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="fa726-310">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="fa726-311">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="fa726-311">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="fa726-312">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="fa726-312">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="fa726-313">Batch</span><span class="sxs-lookup"><span data-stu-id="fa726-313">Batch</span></span>

* <span data-ttu-id="fa726-314">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fa726-314">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="fa726-315">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-315">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="fa726-316">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-316">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="fa726-317">CDN</span><span class="sxs-lookup"><span data-stu-id="fa726-317">CDN</span></span>

* <span data-ttu-id="fa726-318">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fa726-318">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="fa726-319">Cloud</span><span class="sxs-lookup"><span data-stu-id="fa726-319">Cloud</span></span>

* <span data-ttu-id="fa726-320">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="fa726-320">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="fa726-321">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa726-321">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="fa726-322">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fa726-322">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="fa726-323">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="fa726-323">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="fa726-324">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fa726-324">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fa726-325">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fa726-325">CosmosDB</span></span>

* <span data-ttu-id="fa726-326">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="fa726-326">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="fa726-327">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-327">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fa726-328">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fa726-328">Data Lake Analytics</span></span>

* <span data-ttu-id="fa726-329">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-329">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="fa726-330">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-330">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="fa726-331">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-331">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fa726-332">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-332">Data Lake Store</span></span>

* <span data-ttu-id="fa726-333">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-333">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="fa726-334">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="fa726-334">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="fa726-335">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fa726-335">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="fa726-336">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="fa726-336">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="fa726-337">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="fa726-337">Interactive</span></span>

* <span data-ttu-id="fa726-338">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="fa726-338">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="fa726-339">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="fa726-339">Increased test coverage</span></span>
* <span data-ttu-id="fa726-340">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="fa726-340">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="fa726-341">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="fa726-341">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="fa726-342">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="fa726-342">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="fa726-343">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="fa726-343">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="fa726-344">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="fa726-344">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fa726-345">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-345">Added `--progress` flag</span></span>
* <span data-ttu-id="fa726-346">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-346">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="fa726-347">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="fa726-347">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="fa726-348">IoT</span><span class="sxs-lookup"><span data-stu-id="fa726-348">IoT</span></span>

* <span data-ttu-id="fa726-349">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="fa726-349">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="fa726-350">(3934)</span><span class="sxs-lookup"><span data-stu-id="fa726-350">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="fa726-351">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="fa726-351">Key vault</span></span>

* <span data-ttu-id="fa726-352">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fa726-352">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="fa726-353">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fa726-353">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="fa726-354">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fa726-354">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fa726-355">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fa726-355">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fa726-356">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fa726-356">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="fa726-357">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="fa726-357">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="fa726-358">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fa726-358">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="fa726-359">(3307)</span><span class="sxs-lookup"><span data-stu-id="fa726-359">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="fa726-360">Labor</span><span class="sxs-lookup"><span data-stu-id="fa726-360">Lab</span></span>

* <span data-ttu-id="fa726-361">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-361">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="fa726-362">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-362">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="fa726-363">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fa726-363">Monitor</span></span>

* <span data-ttu-id="fa726-364">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="fa726-364">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="fa726-365">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-365">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="fa726-366">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-366">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="fa726-367">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-367">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="fa726-368">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fa726-368">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="fa726-369">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="fa726-369">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="fa726-370">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="fa726-370">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="fa726-371">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="fa726-371">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="fa726-372">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa726-372">`location` no longer required</span></span>
  * <span data-ttu-id="fa726-373">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="fa726-373">Add name and ID support for target</span></span>
  * <span data-ttu-id="fa726-374">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="fa726-374">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="fa726-375">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="fa726-375">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="fa726-376">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fa726-376">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="fa726-377">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="fa726-377">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="fa726-378">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="fa726-378">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="fa726-379">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-379">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="fa726-380">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-380">Network</span></span>

* <span data-ttu-id="fa726-381">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-381">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="fa726-382">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-382">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="fa726-383">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fa726-383">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="fa726-384">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fa726-384">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="fa726-385">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="fa726-385">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="fa726-386">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-386">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="fa726-387">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="fa726-387">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="fa726-388">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="fa726-388">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="fa726-389">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="fa726-389">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="fa726-390">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="fa726-390">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="fa726-391">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-391">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="fa726-392">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-392">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="fa726-393">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="fa726-393">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="fa726-394">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-394">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="fa726-395">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-395">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="fa726-396">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-396">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="fa726-397">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-397">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="fa726-398">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="fa726-398">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="fa726-399">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-399">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="fa726-400">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fa726-400">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="fa726-401">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="fa726-401">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="fa726-402">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fa726-402">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="fa726-403">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="fa726-403">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="fa726-404">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fa726-404">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="fa726-405">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fa726-405">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="fa726-406">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fa726-406">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="fa726-407">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fa726-407">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="fa726-408">Profil</span><span class="sxs-lookup"><span data-stu-id="fa726-408">Profile</span></span>

* <span data-ttu-id="fa726-409">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="fa726-409">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="fa726-410">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="fa726-410">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="fa726-411">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="fa726-411">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="fa726-412">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-412">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="fa726-413">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="fa726-413">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="fa726-414">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fa726-414">RDBMS</span></span>

* <span data-ttu-id="fa726-415">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="fa726-415">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="fa726-416">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="fa726-416">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="fa726-417">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="fa726-417">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="fa726-418">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="fa726-418">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="fa726-419">Ressource</span><span class="sxs-lookup"><span data-stu-id="fa726-419">Resource</span></span>

* <span data-ttu-id="fa726-420">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="fa726-420">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="fa726-421">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="fa726-421">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="fa726-422">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="fa726-422">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="fa726-423">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="fa726-423">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="fa726-424">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="fa726-424">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="fa726-425">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="fa726-425">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="fa726-426">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="fa726-426">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="fa726-427">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-427">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="fa726-428">Rolle</span><span class="sxs-lookup"><span data-stu-id="fa726-428">Role</span></span>

* <span data-ttu-id="fa726-429">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="fa726-429">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="fa726-430">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="fa726-430">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="fa726-431">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="fa726-431">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="fa726-432">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="fa726-432">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="fa726-433">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-433">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fa726-434">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fa726-434">Service Fabric</span></span>
* <span data-ttu-id="fa726-435">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="fa726-435">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="fa726-436">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="fa726-436">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="fa726-437">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="fa726-437">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="fa726-438">SQL</span><span class="sxs-lookup"><span data-stu-id="fa726-438">SQL</span></span>

* <span data-ttu-id="fa726-439">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-439">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="fa726-440">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="fa726-440">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="fa726-441">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-441">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-442">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-442">Storage</span></span>

* <span data-ttu-id="fa726-443">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="fa726-443">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="fa726-444">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fa726-444">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="fa726-445">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="fa726-445">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="fa726-446">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="fa726-446">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="fa726-447">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="fa726-447">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="fa726-448">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="fa726-448">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-449">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-449">VM</span></span>

* <span data-ttu-id="fa726-450">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="fa726-450">Support configuring nsg</span></span>
* <span data-ttu-id="fa726-451">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="fa726-451">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="fa726-452">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="fa726-452">Support managed service identities</span></span>
* <span data-ttu-id="fa726-453">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="fa726-453">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="fa726-454">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="fa726-454">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="fa726-455">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-455">May 10, 2017</span></span>

<span data-ttu-id="fa726-456">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="fa726-456">Version 2.0.6</span></span>

* <span data-ttu-id="fa726-457">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="fa726-457">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="fa726-458">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="fa726-458">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="fa726-459">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="fa726-459">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="fa726-460">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="fa726-460">Include Cognitive Services module.</span></span>
* <span data-ttu-id="fa726-461">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="fa726-461">Include Service Fabric module.</span></span>
* <span data-ttu-id="fa726-462">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="fa726-462">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="fa726-463">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="fa726-463">Add support for CDN commands.</span></span>
* <span data-ttu-id="fa726-464">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="fa726-464">Remove Container module.</span></span>
* <span data-ttu-id="fa726-465">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="fa726-465">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="fa726-466">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fa726-466">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="fa726-467">Core</span><span class="sxs-lookup"><span data-stu-id="fa726-467">Core</span></span>

* <span data-ttu-id="fa726-468">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="fa726-468">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="fa726-469">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="fa726-469">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="fa726-470">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="fa726-470">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="fa726-471">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="fa726-471">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="fa726-472">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="fa726-472">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="fa726-473">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="fa726-473">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="fa726-474">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="fa726-474">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="fa726-475">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="fa726-475">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="fa726-476">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="fa726-476">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="fa726-477">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="fa726-477">core: Improved performance</span></span>
* <span data-ttu-id="fa726-478">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="fa726-478">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="fa726-479">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="fa726-479">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="fa726-480">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-480">ACS</span></span>

* <span data-ttu-id="fa726-481">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa726-481">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="fa726-482">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="fa726-482">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="fa726-483">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="fa726-483">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="fa726-484">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="fa726-484">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="fa726-485">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-485">AppService</span></span>

* <span data-ttu-id="fa726-486">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="fa726-486">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="fa726-487">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="fa726-487">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="fa726-488">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="fa726-488">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="fa726-489">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="fa726-489">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="fa726-490">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="fa726-490">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="fa726-491">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="fa726-491">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="fa726-492">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="fa726-492">support slot swap with preview</span></span>
* <span data-ttu-id="fa726-493">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="fa726-493">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="fa726-494">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="fa726-494">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fa726-495">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fa726-495">CosmosDB</span></span>

* <span data-ttu-id="fa726-496">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="fa726-496">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="fa726-497">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="fa726-497">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="fa726-498">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="fa726-498">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="fa726-499">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="fa726-499">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fa726-500">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fa726-500">Data Lake Analytics</span></span>

* <span data-ttu-id="fa726-501">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="fa726-501">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="fa726-502">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="fa726-502">Add support for new catalog item type: package.</span></span> <span data-ttu-id="fa726-503">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="fa726-503">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="fa726-504">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="fa726-504">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="fa726-505">Table</span><span class="sxs-lookup"><span data-stu-id="fa726-505">Table</span></span>
  * <span data-ttu-id="fa726-506">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="fa726-506">Table valued function</span></span>
  * <span data-ttu-id="fa726-507">Sicht</span><span class="sxs-lookup"><span data-stu-id="fa726-507">View</span></span>
  * <span data-ttu-id="fa726-508">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="fa726-508">Table Statistics.</span></span> <span data-ttu-id="fa726-509">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="fa726-509">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fa726-510">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fa726-510">Data Lake Store</span></span>

* <span data-ttu-id="fa726-511">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="fa726-511">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="fa726-512">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fa726-512">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="fa726-513">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="fa726-513">missed help for access show.</span></span> <span data-ttu-id="fa726-514">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fa726-514">adding it.</span></span> <span data-ttu-id="fa726-515">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="fa726-515">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="fa726-516">Suchen</span><span class="sxs-lookup"><span data-stu-id="fa726-516">Find</span></span>

* <span data-ttu-id="fa726-517">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="fa726-517">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="fa726-518">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa726-518">KeyVault</span></span>

* <span data-ttu-id="fa726-519">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="fa726-519">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="fa726-520">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="fa726-520">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="fa726-521">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="fa726-521">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="fa726-522">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="fa726-522">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="fa726-523">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="fa726-523">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="fa726-524">Labor</span><span class="sxs-lookup"><span data-stu-id="fa726-524">Lab</span></span>

* <span data-ttu-id="fa726-525">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="fa726-525">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="fa726-526">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="fa726-526">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="fa726-527">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="fa726-527">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="fa726-528">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="fa726-528">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="fa726-529">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="fa726-529">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="fa726-530">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fa726-530">Monitor</span></span>

* <span data-ttu-id="fa726-531">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="fa726-531">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="fa726-532">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="fa726-532">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="fa726-533">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-533">Network</span></span>

* <span data-ttu-id="fa726-534">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="fa726-534">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="fa726-535">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="fa726-535">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="fa726-536">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="fa726-536">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="fa726-537">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="fa726-537">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="fa726-538">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="fa726-538">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="fa726-539">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="fa726-539">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="fa726-540">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="fa726-540">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="fa726-541">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="fa726-541">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="fa726-542">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="fa726-542">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="fa726-543">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="fa726-543">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="fa726-544">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="fa726-544">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="fa726-545">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="fa726-545">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="fa726-546">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="fa726-546">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="fa726-547">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="fa726-547">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="fa726-548">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fa726-548">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="fa726-549">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="fa726-549">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="fa726-550">Profil</span><span class="sxs-lookup"><span data-stu-id="fa726-550">Profile</span></span>

* <span data-ttu-id="fa726-551">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="fa726-551">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="fa726-552">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="fa726-552">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="fa726-553">Redis</span><span class="sxs-lookup"><span data-stu-id="fa726-553">Redis</span></span>

* <span data-ttu-id="fa726-554">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="fa726-554">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="fa726-555">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="fa726-555">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="fa726-556">Ressource</span><span class="sxs-lookup"><span data-stu-id="fa726-556">Resource</span></span>

* <span data-ttu-id="fa726-557">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="fa726-557">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="fa726-558">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="fa726-558">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="fa726-559">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="fa726-559">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="fa726-560">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="fa726-560">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="fa726-561">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="fa726-561">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="fa726-562">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="fa726-562">Add docs for az lock update.</span></span> <span data-ttu-id="fa726-563">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="fa726-563">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="fa726-564">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="fa726-564">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="fa726-565">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="fa726-565">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="fa726-566">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="fa726-566">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="fa726-567">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="fa726-567">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="fa726-568">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="fa726-568">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="fa726-569">Rolle</span><span class="sxs-lookup"><span data-stu-id="fa726-569">Role</span></span>

* <span data-ttu-id="fa726-570">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="fa726-570">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="fa726-571">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="fa726-571">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="fa726-572">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="fa726-572">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="fa726-573">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="fa726-573">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="fa726-574">SQL</span><span class="sxs-lookup"><span data-stu-id="fa726-574">SQL</span></span>

* <span data-ttu-id="fa726-575">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="fa726-575">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="fa726-576">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="fa726-576">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="fa726-577">Speicher</span><span class="sxs-lookup"><span data-stu-id="fa726-577">Storage</span></span>

* <span data-ttu-id="fa726-578">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="fa726-578">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="fa726-579">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="fa726-579">Add support for incremental blob copy</span></span>
* <span data-ttu-id="fa726-580">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="fa726-580">Add support for large block blob upload</span></span>
* <span data-ttu-id="fa726-581">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="fa726-581">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-582">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-582">VM</span></span>

* <span data-ttu-id="fa726-583">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="fa726-583">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="fa726-584">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="fa726-584">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="fa726-585">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="fa726-585">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="fa726-586">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="fa726-586">az vm/vmss disk</span></span>
  3. <span data-ttu-id="fa726-587">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="fa726-587">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="fa726-588">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="fa726-588">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="fa726-589">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="fa726-589">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="fa726-590">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-590">April 3, 2017</span></span>

<span data-ttu-id="fa726-591">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="fa726-591">Version 2.0.2</span></span>

<span data-ttu-id="fa726-592">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="fa726-592">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="fa726-593">Core</span><span class="sxs-lookup"><span data-stu-id="fa726-593">Core</span></span>

* <span data-ttu-id="fa726-594">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="fa726-594">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="fa726-595">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="fa726-595">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="fa726-596">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="fa726-596">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="fa726-597">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fa726-597">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fa726-598">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="fa726-598">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="fa726-599">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="fa726-599">Add prompting for missing template parameters.</span></span> <span data-ttu-id="fa726-600">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="fa726-600">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="fa726-601">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="fa726-601">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="fa726-602">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="fa726-602">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="fa726-603">ACS</span><span class="sxs-lookup"><span data-stu-id="fa726-603">ACS</span></span>

* <span data-ttu-id="fa726-604">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="fa726-604">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="fa726-605">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="fa726-605">Add support for ssh key password prompting.</span></span> <span data-ttu-id="fa726-606">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="fa726-606">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="fa726-607">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="fa726-607">Add support for windows clusters.</span></span> <span data-ttu-id="fa726-608">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="fa726-608">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="fa726-609">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="fa726-609">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="fa726-610">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="fa726-610">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="fa726-611">AppService</span><span class="sxs-lookup"><span data-stu-id="fa726-611">AppService</span></span>

* <span data-ttu-id="fa726-612">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="fa726-612">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="fa726-613">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="fa726-613">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="fa726-614">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="fa726-614">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="fa726-615">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="fa726-615">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="fa726-616">DataLake</span><span class="sxs-lookup"><span data-stu-id="fa726-616">DataLake</span></span>

* <span data-ttu-id="fa726-617">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="fa726-617">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="fa726-618">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="fa726-618">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="fa726-619">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="fa726-619">DocuemntDB</span></span>

* <span data-ttu-id="fa726-620">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="fa726-620">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="fa726-621">VM</span><span class="sxs-lookup"><span data-stu-id="fa726-621">VM</span></span>

* <span data-ttu-id="fa726-622">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="fa726-622">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="fa726-623">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="fa726-623">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="fa726-624">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="fa726-624">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="fa726-625">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fa726-625">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fa726-626">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="fa726-626">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="fa726-627">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="fa726-627">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="fa726-628">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="fa726-628">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="fa726-629">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="fa726-629">February 27, 2017</span></span>

<span data-ttu-id="fa726-630">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="fa726-630">Version 2.0.0</span></span>

<span data-ttu-id="fa726-631">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="fa726-631">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="fa726-632">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="fa726-632">General availability applies to these command modules:</span></span>
- <span data-ttu-id="fa726-633">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="fa726-633">Container Service (acs)</span></span>
- <span data-ttu-id="fa726-634">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="fa726-634">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="fa726-635">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fa726-635">Networking</span></span>
- <span data-ttu-id="fa726-636">Storage</span><span class="sxs-lookup"><span data-stu-id="fa726-636">Storage</span></span>

<span data-ttu-id="fa726-637">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fa726-637">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="fa726-638">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="fa726-638">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="fa726-639">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="fa726-639">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="fa726-640">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="fa726-640">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="fa726-641">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="fa726-641">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="fa726-642">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="fa726-642">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="fa726-643">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="fa726-643">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="fa726-644">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="fa726-644">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="fa726-645">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="fa726-645">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="fa726-646">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="fa726-646">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="fa726-647">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="fa726-647">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="fa726-648">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="fa726-648">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="fa726-649">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="fa726-649">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="fa726-650">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="fa726-650">Provide feedback from the command line with the `az feedback` command.</span></span>

