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
ms.openlocfilehash: ad30efeb7efafcc5816160ee130665d37adb62c6
ms.sourcegitcommit: e866977985ba0286fa05f41729dd7e7d9ce86f8e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/13/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="4f4a2-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="4f4a2-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-11-2017"></a><span data-ttu-id="4f4a2-105">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-105">September 11, 2017</span></span>

<span data-ttu-id="4f4a2-106">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4f4a2-106">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4f4a2-107">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-107">Core</span></span>

* <span data-ttu-id="4f4a2-108">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-108">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4f4a2-109">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="4f4a2-109">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-110">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-110">Acs</span></span>

* <span data-ttu-id="4f4a2-111">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-111">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4f4a2-112">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-112">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-113">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-113">Appservice</span></span>

* <span data-ttu-id="4f4a2-114">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="4f4a2-114">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4f4a2-115">CDN</span><span class="sxs-lookup"><span data-stu-id="4f4a2-115">CDN</span></span>

* <span data-ttu-id="4f4a2-116">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-116">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="4f4a2-117">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4f4a2-117">Extension</span></span>

* <span data-ttu-id="4f4a2-118">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-118">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-119">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4f4a2-119">Keyvault</span></span>

* <span data-ttu-id="4f4a2-120">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="4f4a2-120">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-121">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-121">Network</span></span>

* <span data-ttu-id="4f4a2-122">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-122">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4f4a2-123">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-123">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4f4a2-124">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-124">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4f4a2-125">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4f4a2-126">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-126">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-127">Ressource</span><span class="sxs-lookup"><span data-stu-id="4f4a2-127">Resource</span></span>

* <span data-ttu-id="4f4a2-128">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-128">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4f4a2-129">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-129">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4f4a2-130">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-130">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4f4a2-131">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="4f4a2-131">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-132">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-132">SQL</span></span>

* <span data-ttu-id="4f4a2-133">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-133">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-134">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-134">VM</span></span>

* <span data-ttu-id="4f4a2-135">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4f4a2-135">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4f4a2-136">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-136">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4f4a2-137">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-137">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4f4a2-138">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-138">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4f4a2-139">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-139">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4f4a2-140">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-140">August 31, 2017</span></span>

<span data-ttu-id="4f4a2-141">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4f4a2-141">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4f4a2-142">Keyvault</span></span>

* <span data-ttu-id="4f4a2-143">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-143">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4f4a2-144">Sf</span><span class="sxs-lookup"><span data-stu-id="4f4a2-144">Sf</span></span>

* <span data-ttu-id="4f4a2-145">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-145">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-146">Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-146">Storage</span></span>

* <span data-ttu-id="4f4a2-147">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-147">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4f4a2-148">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="4f4a2-148">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4f4a2-149">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-149">August 28, 2017</span></span>

<span data-ttu-id="4f4a2-150">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4f4a2-150">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4f4a2-151">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-151">CLI</span></span>

* <span data-ttu-id="4f4a2-152">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-152">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-153">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-153">ACS</span></span>

* <span data-ttu-id="4f4a2-154">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-154">Corrected preview regions.</span></span>
* <span data-ttu-id="4f4a2-155">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-155">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="4f4a2-156">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-156">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-157">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-157">Appservice</span></span>

* <span data-ttu-id="4f4a2-158">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-158">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4f4a2-159">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-159">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4f4a2-160">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-160">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4f4a2-161">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-161">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4f4a2-162">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-162">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4f4a2-163">IoT</span><span class="sxs-lookup"><span data-stu-id="4f4a2-163">IoT</span></span>

* <span data-ttu-id="4f4a2-164">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4f4a2-164">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-165">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-165">Network</span></span>

* <span data-ttu-id="4f4a2-166">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-166">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4f4a2-167">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-167">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4f4a2-168">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-168">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4f4a2-169">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-169">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4f4a2-170">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-170">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-171">Profil</span><span class="sxs-lookup"><span data-stu-id="4f4a2-171">Profile</span></span>

* <span data-ttu-id="4f4a2-172">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-172">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4f4a2-173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4f4a2-173">Service Fabric</span></span>

* <span data-ttu-id="4f4a2-174">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4f4a2-174">Preview release</span></span>
* <span data-ttu-id="4f4a2-175">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-175">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4f4a2-176">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-176">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4f4a2-177">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-177">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-178">Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-178">Storage</span></span>

* <span data-ttu-id="4f4a2-179">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-179">Enabled setting blob tier</span></span>
* <span data-ttu-id="4f4a2-180">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-180">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4f4a2-181">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-181">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="4f4a2-182">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-182">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4f4a2-183">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-183">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4f4a2-184">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-184">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-185">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-185">VM</span></span>

* <span data-ttu-id="4f4a2-186">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-186">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4f4a2-187">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-187">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="4f4a2-188">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-188">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="4f4a2-189">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-189">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4f4a2-190">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-190">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4f4a2-191">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4f4a2-191">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4f4a2-192">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-192">August 15, 2017</span></span>

<span data-ttu-id="4f4a2-193">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4f4a2-193">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-194">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-194">ACS</span></span>

* <span data-ttu-id="4f4a2-195">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-195">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-196">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-196">Appservice</span></span>

* <span data-ttu-id="4f4a2-197">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-197">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4f4a2-198">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4f4a2-198">Event Grid</span></span>

* <span data-ttu-id="4f4a2-199">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-199">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4f4a2-200">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-200">August 11, 2017</span></span>

<span data-ttu-id="4f4a2-201">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4f4a2-201">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-202">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-202">ACS</span></span>

* <span data-ttu-id="4f4a2-203">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-203">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4f4a2-204">Batch</span><span class="sxs-lookup"><span data-stu-id="4f4a2-204">Batch</span></span>

* <span data-ttu-id="4f4a2-205">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-205">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4f4a2-206">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-206">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4f4a2-207">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-207">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4f4a2-208">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-208">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4f4a2-209">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="4f4a2-209">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4f4a2-210">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-210">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4f4a2-211">Komponente</span><span class="sxs-lookup"><span data-stu-id="4f4a2-211">Component</span></span>

* <span data-ttu-id="4f4a2-212">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-212">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4f4a2-213">Container</span><span class="sxs-lookup"><span data-stu-id="4f4a2-213">Container</span></span>

* <span data-ttu-id="4f4a2-214">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="4f4a2-214">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-215">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-215">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-216">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-216">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4f4a2-217">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4f4a2-217">Event Grid</span></span>

* <span data-ttu-id="4f4a2-218">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4f4a2-218">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-219">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-219">Network</span></span>

* <span data-ttu-id="4f4a2-220">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-220">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4f4a2-221">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="4f4a2-221">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4f4a2-222">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="4f4a2-222">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4f4a2-223">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-223">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-224">Profil</span><span class="sxs-lookup"><span data-stu-id="4f4a2-224">Profile</span></span>

* <span data-ttu-id="4f4a2-225">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="4f4a2-225">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-226">Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-226">Storage</span></span>

* <span data-ttu-id="4f4a2-227">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-227">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-228">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-228">VM</span></span>

* <span data-ttu-id="4f4a2-229">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-229">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4f4a2-230">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-230">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4f4a2-231">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-231">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4f4a2-232">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="4f4a2-232">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4f4a2-233">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-233">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4f4a2-234">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-234">July 28, 2017</span></span>

<span data-ttu-id="4f4a2-235">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4f4a2-235">Version 2.0.12</span></span>

* <span data-ttu-id="4f4a2-236">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-236">Added container commands</span></span>
* <span data-ttu-id="4f4a2-237">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-237">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-238">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-238">Core</span></span>

* <span data-ttu-id="4f4a2-239">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-239">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4f4a2-240">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-240">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4f4a2-241">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="4f4a2-241">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4f4a2-242">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-242">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4f4a2-243">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-243">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4f4a2-244">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-244">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4f4a2-245">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-245">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4f4a2-246">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-246">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4f4a2-247">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-247">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4f4a2-248">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="4f4a2-248">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4f4a2-249">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="4f4a2-249">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4f4a2-250">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-250">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4f4a2-251">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-251">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4f4a2-252">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-252">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4f4a2-253">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4f4a2-253">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4f4a2-254">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-254">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4f4a2-255">ACR</span><span class="sxs-lookup"><span data-stu-id="4f4a2-255">ACR</span></span>

* <span data-ttu-id="4f4a2-256">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-256">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4f4a2-257">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-257">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4f4a2-258">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-258">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4f4a2-259">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-259">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4f4a2-260">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-260">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4f4a2-261">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-261">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-262">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-262">ACS</span></span>

* <span data-ttu-id="4f4a2-263">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="4f4a2-263">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-264">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-264">Appservice</span></span>

* <span data-ttu-id="4f4a2-265">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="4f4a2-265">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4f4a2-266">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="4f4a2-266">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4f4a2-267">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-267">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4f4a2-268">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-268">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4f4a2-269">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-269">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4f4a2-270">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-270">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4f4a2-271">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-271">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4f4a2-272">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-272">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4f4a2-273">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-273">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4f4a2-274">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-274">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4f4a2-275">Batch</span><span class="sxs-lookup"><span data-stu-id="4f4a2-275">Batch</span></span>

* <span data-ttu-id="4f4a2-276">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-276">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4f4a2-277">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-277">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4f4a2-278">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-278">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4f4a2-279">CDN</span><span class="sxs-lookup"><span data-stu-id="4f4a2-279">CDN</span></span>

* <span data-ttu-id="4f4a2-280">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="4f4a2-280">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="4f4a2-281">Cloud</span><span class="sxs-lookup"><span data-stu-id="4f4a2-281">Cloud</span></span>

* <span data-ttu-id="4f4a2-282">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-282">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4f4a2-283">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f4a2-283">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4f4a2-284">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-284">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4f4a2-285">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="4f4a2-285">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4f4a2-286">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-286">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4f4a2-287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-287">CosmosDB</span></span>

* <span data-ttu-id="4f4a2-288">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-288">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4f4a2-289">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-289">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4f4a2-290">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4f4a2-290">Data Lake Analytics</span></span>

* <span data-ttu-id="4f4a2-291">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-291">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4f4a2-292">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-292">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4f4a2-293">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-293">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-294">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-294">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-295">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-295">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4f4a2-296">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="4f4a2-296">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4f4a2-297">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-297">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4f4a2-298">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-298">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4f4a2-299">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="4f4a2-299">Interactive</span></span>

* <span data-ttu-id="4f4a2-300">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-300">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4f4a2-301">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-301">Increased test coverage</span></span>
* <span data-ttu-id="4f4a2-302">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="4f4a2-302">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4f4a2-303">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-303">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4f4a2-304">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-304">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4f4a2-305">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-305">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4f4a2-306">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-306">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4f4a2-307">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-307">Added `--progress` flag</span></span>
* <span data-ttu-id="4f4a2-308">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-308">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4f4a2-309">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-309">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4f4a2-310">IoT</span><span class="sxs-lookup"><span data-stu-id="4f4a2-310">IoT</span></span>

* <span data-ttu-id="4f4a2-311">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4f4a2-311">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4f4a2-312">(3934)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-312">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4f4a2-313">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="4f4a2-313">Key vault</span></span>

* <span data-ttu-id="4f4a2-314">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-314">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4f4a2-315">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-315">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-316">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-316">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-317">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-317">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-318">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-318">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4f4a2-319">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-319">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4f4a2-320">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-320">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4f4a2-321">(3307)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-321">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4f4a2-322">Labor</span><span class="sxs-lookup"><span data-stu-id="4f4a2-322">Lab</span></span>

* <span data-ttu-id="4f4a2-323">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-323">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4f4a2-324">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-324">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4f4a2-325">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-325">Monitor</span></span>

* <span data-ttu-id="4f4a2-326">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-326">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4f4a2-327">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-327">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4f4a2-328">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-328">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4f4a2-329">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-329">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4f4a2-330">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-330">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4f4a2-331">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-331">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4f4a2-332">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-332">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4f4a2-333">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-333">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4f4a2-334">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f4a2-334">`location` no longer required</span></span>
  * <span data-ttu-id="4f4a2-335">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="4f4a2-335">Add name and ID support for target</span></span>
  * <span data-ttu-id="4f4a2-336">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-336">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4f4a2-337">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-337">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4f4a2-338">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-338">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4f4a2-339">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="4f4a2-339">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4f4a2-340">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-340">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4f4a2-341">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-341">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-342">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-342">Network</span></span>

* <span data-ttu-id="4f4a2-343">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-343">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4f4a2-344">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-344">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4f4a2-345">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4f4a2-345">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4f4a2-346">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4f4a2-346">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4f4a2-347">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="4f4a2-347">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4f4a2-348">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-348">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4f4a2-349">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-349">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4f4a2-350">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-350">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4f4a2-351">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-351">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4f4a2-352">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-352">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4f4a2-353">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-353">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4f4a2-354">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-354">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4f4a2-355">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-355">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4f4a2-356">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-356">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4f4a2-357">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-357">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4f4a2-358">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-358">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4f4a2-359">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-359">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4f4a2-360">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="4f4a2-360">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4f4a2-361">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-361">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4f4a2-362">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-362">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4f4a2-363">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-363">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4f4a2-364">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-364">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4f4a2-365">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-365">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4f4a2-366">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-366">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-367">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-367">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-368">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-368">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-369">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-369">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-370">Profil</span><span class="sxs-lookup"><span data-stu-id="4f4a2-370">Profile</span></span>

* <span data-ttu-id="4f4a2-371">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="4f4a2-371">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4f4a2-372">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="4f4a2-372">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4f4a2-373">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-373">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4f4a2-374">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-374">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4f4a2-375">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="4f4a2-375">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4f4a2-376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-376">RDBMS</span></span>

* <span data-ttu-id="4f4a2-377">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-377">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4f4a2-378">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-378">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4f4a2-379">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-379">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4f4a2-380">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-380">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-381">Ressource</span><span class="sxs-lookup"><span data-stu-id="4f4a2-381">Resource</span></span>

* <span data-ttu-id="4f4a2-382">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-382">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4f4a2-383">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="4f4a2-383">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4f4a2-384">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-384">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4f4a2-385">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-385">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4f4a2-386">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-386">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4f4a2-387">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-387">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4f4a2-388">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-388">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4f4a2-389">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-389">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4f4a2-390">Rolle</span><span class="sxs-lookup"><span data-stu-id="4f4a2-390">Role</span></span>

* <span data-ttu-id="4f4a2-391">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-391">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4f4a2-392">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-392">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4f4a2-393">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="4f4a2-393">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4f4a2-394">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-394">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4f4a2-395">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-395">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4f4a2-396">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4f4a2-396">Service Fabric</span></span>
* <span data-ttu-id="4f4a2-397">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-397">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4f4a2-398">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-398">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4f4a2-399">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-399">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-400">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-400">SQL</span></span>

* <span data-ttu-id="4f4a2-401">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-401">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4f4a2-402">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-402">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4f4a2-403">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-403">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-404">Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-404">Storage</span></span>

* <span data-ttu-id="4f4a2-405">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-405">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4f4a2-406">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-406">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4f4a2-407">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-407">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4f4a2-408">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-408">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="4f4a2-409">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-409">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="4f4a2-410">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-410">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-411">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-411">VM</span></span>

* <span data-ttu-id="4f4a2-412">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="4f4a2-412">Support configuring nsg</span></span>
* <span data-ttu-id="4f4a2-413">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="4f4a2-413">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4f4a2-414">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-414">Support managed service identities</span></span>
* <span data-ttu-id="4f4a2-415">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-415">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="4f4a2-416">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-416">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4f4a2-417">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-417">May 10, 2017</span></span>

<span data-ttu-id="4f4a2-418">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4f4a2-418">Version 2.0.6</span></span>

* <span data-ttu-id="4f4a2-419">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-419">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4f4a2-420">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-420">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4f4a2-421">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="4f4a2-421">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="4f4a2-422">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-422">Include Cognitive Services module.</span></span>
* <span data-ttu-id="4f4a2-423">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-423">Include Service Fabric module.</span></span>
* <span data-ttu-id="4f4a2-424">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-424">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="4f4a2-425">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="4f4a2-425">Add support for CDN commands.</span></span>
* <span data-ttu-id="4f4a2-426">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-426">Remove Container module.</span></span>
* <span data-ttu-id="4f4a2-427">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-427">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4f4a2-428">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-428">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-429">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-429">Core</span></span>

* <span data-ttu-id="4f4a2-430">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-430">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="4f4a2-431">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-431">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4f4a2-432">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-432">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4f4a2-433">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-433">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4f4a2-434">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-434">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4f4a2-435">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-435">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4f4a2-436">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-436">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4f4a2-437">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-437">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4f4a2-438">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-438">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4f4a2-439">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-439">core: Improved performance</span></span>
* <span data-ttu-id="4f4a2-440">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-440">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4f4a2-441">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="4f4a2-441">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-442">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-442">ACS</span></span>

* <span data-ttu-id="4f4a2-443">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f4a2-443">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4f4a2-444">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-444">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4f4a2-445">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-445">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4f4a2-446">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-446">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-447">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-447">AppService</span></span>

* <span data-ttu-id="4f4a2-448">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-448">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4f4a2-449">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-449">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4f4a2-450">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-450">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4f4a2-451">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="4f4a2-451">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4f4a2-452">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-452">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4f4a2-453">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-453">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4f4a2-454">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="4f4a2-454">support slot swap with preview</span></span>
* <span data-ttu-id="4f4a2-455">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-455">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4f4a2-456">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-456">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4f4a2-457">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-457">CosmosDB</span></span>

* <span data-ttu-id="4f4a2-458">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-458">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="4f4a2-459">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-459">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4f4a2-460">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-460">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4f4a2-461">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="4f4a2-461">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4f4a2-462">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4f4a2-462">Data Lake Analytics</span></span>

* <span data-ttu-id="4f4a2-463">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="4f4a2-463">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="4f4a2-464">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-464">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4f4a2-465">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-465">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4f4a2-466">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="4f4a2-466">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4f4a2-467">Table</span><span class="sxs-lookup"><span data-stu-id="4f4a2-467">Table</span></span>
  * <span data-ttu-id="4f4a2-468">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="4f4a2-468">Table valued function</span></span>
  * <span data-ttu-id="4f4a2-469">Sicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-469">View</span></span>
  * <span data-ttu-id="4f4a2-470">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-470">Table Statistics.</span></span> <span data-ttu-id="4f4a2-471">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-471">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-472">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4f4a2-472">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-473">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="4f4a2-473">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="4f4a2-474">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-474">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4f4a2-475">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="4f4a2-475">missed help for access show.</span></span> <span data-ttu-id="4f4a2-476">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4f4a2-476">adding it.</span></span> <span data-ttu-id="4f4a2-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4f4a2-478">Suchen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-478">Find</span></span>

* <span data-ttu-id="4f4a2-479">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="4f4a2-479">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4f4a2-480">KeyVault</span></span>

* <span data-ttu-id="4f4a2-481">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-481">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4f4a2-482">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-482">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="4f4a2-483">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="4f4a2-483">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4f4a2-484">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="4f4a2-484">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="4f4a2-485">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-485">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4f4a2-486">Labor</span><span class="sxs-lookup"><span data-stu-id="4f4a2-486">Lab</span></span>

* <span data-ttu-id="4f4a2-487">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="4f4a2-487">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="4f4a2-488">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="4f4a2-488">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="4f4a2-489">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="4f4a2-489">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="4f4a2-490">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="4f4a2-490">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="4f4a2-491">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="4f4a2-491">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="4f4a2-492">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-492">Monitor</span></span>

* <span data-ttu-id="4f4a2-493">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-493">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4f4a2-494">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-494">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-495">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-495">Network</span></span>

* <span data-ttu-id="4f4a2-496">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-496">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="4f4a2-497">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-497">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="4f4a2-498">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="4f4a2-498">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="4f4a2-499">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-499">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="4f4a2-500">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="4f4a2-500">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="4f4a2-501">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="4f4a2-501">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="4f4a2-502">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-502">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="4f4a2-503">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-503">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="4f4a2-504">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-504">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="4f4a2-505">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="4f4a2-505">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4f4a2-506">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-506">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="4f4a2-507">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-507">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="4f4a2-508">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="4f4a2-508">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="4f4a2-509">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4f4a2-509">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="4f4a2-510">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4f4a2-510">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="4f4a2-511">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-511">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-512">Profil</span><span class="sxs-lookup"><span data-stu-id="4f4a2-512">Profile</span></span>

* <span data-ttu-id="4f4a2-513">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-513">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4f4a2-514">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-514">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4f4a2-515">Redis</span><span class="sxs-lookup"><span data-stu-id="4f4a2-515">Redis</span></span>

* <span data-ttu-id="4f4a2-516">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="4f4a2-516">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4f4a2-517">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-517">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-518">Ressource</span><span class="sxs-lookup"><span data-stu-id="4f4a2-518">Resource</span></span>

* <span data-ttu-id="4f4a2-519">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-519">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4f4a2-520">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-520">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4f4a2-521">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-521">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4f4a2-522">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="4f4a2-522">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4f4a2-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4f4a2-524">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-524">Add docs for az lock update.</span></span> <span data-ttu-id="4f4a2-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4f4a2-526">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-526">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4f4a2-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4f4a2-528">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="4f4a2-528">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4f4a2-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4f4a2-530">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-530">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4f4a2-531">Rolle</span><span class="sxs-lookup"><span data-stu-id="4f4a2-531">Role</span></span>

* <span data-ttu-id="4f4a2-532">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-532">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4f4a2-533">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-533">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4f4a2-534">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-534">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4f4a2-535">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="4f4a2-535">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-536">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-536">SQL</span></span>

* <span data-ttu-id="4f4a2-537">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-537">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="4f4a2-538">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-538">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-539">Speicher</span><span class="sxs-lookup"><span data-stu-id="4f4a2-539">Storage</span></span>

* <span data-ttu-id="4f4a2-540">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-540">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="4f4a2-541">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="4f4a2-541">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4f4a2-542">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="4f4a2-542">Add support for large block blob upload</span></span>
* <span data-ttu-id="4f4a2-543">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="4f4a2-543">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-544">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-544">VM</span></span>

* <span data-ttu-id="4f4a2-545">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="4f4a2-545">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4f4a2-546">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-546">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4f4a2-547">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4f4a2-547">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4f4a2-548">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-548">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4f4a2-549">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-549">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4f4a2-550">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="4f4a2-550">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4f4a2-551">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-551">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4f4a2-552">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-552">April 3, 2017</span></span>

<span data-ttu-id="4f4a2-553">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4f4a2-553">Version 2.0.2</span></span>

<span data-ttu-id="4f4a2-554">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-554">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-555">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-555">Core</span></span>

* <span data-ttu-id="4f4a2-556">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="4f4a2-556">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="4f4a2-557">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-557">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4f4a2-558">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-558">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4f4a2-559">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-559">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4f4a2-560">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-560">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4f4a2-561">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="4f4a2-561">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4f4a2-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4f4a2-563">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-563">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4f4a2-564">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="4f4a2-564">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="4f4a2-565">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-565">ACS</span></span>

* <span data-ttu-id="4f4a2-566">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-566">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4f4a2-567">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="4f4a2-567">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4f4a2-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4f4a2-569">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="4f4a2-569">Add support for windows clusters.</span></span> <span data-ttu-id="4f4a2-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4f4a2-571">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="4f4a2-571">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4f4a2-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="4f4a2-573">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-573">AppService</span></span>

* <span data-ttu-id="4f4a2-574">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-574">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4f4a2-575">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-575">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4f4a2-576">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-576">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4f4a2-577">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-577">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="4f4a2-578">DataLake</span><span class="sxs-lookup"><span data-stu-id="4f4a2-578">DataLake</span></span>

* <span data-ttu-id="4f4a2-579">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-579">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="4f4a2-580">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="4f4a2-580">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="4f4a2-581">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-581">DocuemntDB</span></span>

* <span data-ttu-id="4f4a2-582">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-582">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-583">VM</span><span class="sxs-lookup"><span data-stu-id="4f4a2-583">VM</span></span>

* <span data-ttu-id="4f4a2-584">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-584">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4f4a2-585">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-585">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4f4a2-586">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-586">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4f4a2-587">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-587">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4f4a2-588">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-588">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4f4a2-589">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-589">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4f4a2-590">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-590">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4f4a2-591">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="4f4a2-591">February 27, 2017</span></span>

<span data-ttu-id="4f4a2-592">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4f4a2-592">Version 2.0.0</span></span>

<span data-ttu-id="4f4a2-593">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-593">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="4f4a2-594">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-594">General availability applies to these command modules:</span></span>
- <span data-ttu-id="4f4a2-595">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-595">Container Service (acs)</span></span>
- <span data-ttu-id="4f4a2-596">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-596">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4f4a2-597">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-597">Networking</span></span>
- <span data-ttu-id="4f4a2-598">Storage</span><span class="sxs-lookup"><span data-stu-id="4f4a2-598">Storage</span></span>

<span data-ttu-id="4f4a2-599">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-599">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="4f4a2-600">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-600">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="4f4a2-601">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-601">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="4f4a2-602">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-602">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="4f4a2-603">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-603">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="4f4a2-604">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-604">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="4f4a2-605">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-605">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="4f4a2-606">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-606">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="4f4a2-607">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-607">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="4f4a2-608">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-608">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="4f4a2-609">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-609">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4f4a2-610">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-610">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4f4a2-611">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-611">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="4f4a2-612">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-612">Provide feedback from the command line with the `az feedback` command.</span></span>

