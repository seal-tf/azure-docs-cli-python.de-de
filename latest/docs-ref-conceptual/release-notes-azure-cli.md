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
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="6695f-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="6695f-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="6695f-105">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-105">August 28, 2017</span></span>

<span data-ttu-id="6695f-106">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="6695f-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="6695f-107">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="6695f-107">CLI</span></span>

* <span data-ttu-id="6695f-108">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6695f-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="6695f-109">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-109">ACS</span></span>

* <span data-ttu-id="6695f-110">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="6695f-110">Corrected preview regions.</span></span>
* <span data-ttu-id="6695f-111">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="6695f-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="6695f-112">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="6695f-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="6695f-113">AppService</span><span class="sxs-lookup"><span data-stu-id="6695f-113">Appservice</span></span>

* <span data-ttu-id="6695f-114">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="6695f-115">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="6695f-116">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6695f-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="6695f-117">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="6695f-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="6695f-118">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="6695f-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="6695f-119">IoT</span><span class="sxs-lookup"><span data-stu-id="6695f-119">IoT</span></span>

* <span data-ttu-id="6695f-120">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6695f-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="6695f-121">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6695f-121">Network</span></span>

* <span data-ttu-id="6695f-122">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6695f-123">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="6695f-124">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6695f-125">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6695f-126">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="6695f-127">Profil</span><span class="sxs-lookup"><span data-stu-id="6695f-127">Profile</span></span>

* <span data-ttu-id="6695f-128">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6695f-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6695f-129">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6695f-129">Service Fabric</span></span>

* <span data-ttu-id="6695f-130">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6695f-130">Preview release</span></span>
* <span data-ttu-id="6695f-131">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="6695f-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="6695f-132">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="6695f-133">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="6695f-134">Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-134">Storage</span></span>

* <span data-ttu-id="6695f-135">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6695f-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="6695f-136">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="6695f-137">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="6695f-138">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6695f-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="6695f-139">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="6695f-140">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="6695f-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="6695f-141">VM</span><span class="sxs-lookup"><span data-stu-id="6695f-141">VM</span></span>

* <span data-ttu-id="6695f-142">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6695f-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="6695f-143">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6695f-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="6695f-144">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="6695f-145">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6695f-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="6695f-146">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="6695f-147">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6695f-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="6695f-148">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-148">August 15, 2017</span></span>

<span data-ttu-id="6695f-149">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="6695f-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="6695f-150">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-150">ACS</span></span>

* <span data-ttu-id="6695f-151">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="6695f-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="6695f-152">AppService</span><span class="sxs-lookup"><span data-stu-id="6695f-152">Appservice</span></span>

* <span data-ttu-id="6695f-153">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="6695f-154">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6695f-154">Event Grid</span></span>

* <span data-ttu-id="6695f-155">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="6695f-156">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-156">August 11, 2017</span></span>

<span data-ttu-id="6695f-157">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="6695f-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="6695f-158">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-158">ACS</span></span>

* <span data-ttu-id="6695f-159">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="6695f-160">Batch</span><span class="sxs-lookup"><span data-stu-id="6695f-160">Batch</span></span>

* <span data-ttu-id="6695f-161">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6695f-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="6695f-162">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="6695f-163">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="6695f-164">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="6695f-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="6695f-165">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="6695f-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="6695f-166">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="6695f-167">Komponente</span><span class="sxs-lookup"><span data-stu-id="6695f-167">Component</span></span>

* <span data-ttu-id="6695f-168">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="6695f-169">Container</span><span class="sxs-lookup"><span data-stu-id="6695f-169">Container</span></span>

* <span data-ttu-id="6695f-170">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="6695f-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="6695f-171">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-171">Data Lake Store</span></span>

* <span data-ttu-id="6695f-172">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6695f-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="6695f-173">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6695f-173">Event Grid</span></span>

* <span data-ttu-id="6695f-174">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6695f-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="6695f-175">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6695f-175">Network</span></span>

* <span data-ttu-id="6695f-176">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="6695f-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="6695f-177">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6695f-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="6695f-178">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="6695f-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="6695f-179">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="6695f-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="6695f-180">Profil</span><span class="sxs-lookup"><span data-stu-id="6695f-180">Profile</span></span>

* <span data-ttu-id="6695f-181">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="6695f-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="6695f-182">Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-182">Storage</span></span>

* <span data-ttu-id="6695f-183">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6695f-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="6695f-184">VM</span><span class="sxs-lookup"><span data-stu-id="6695f-184">VM</span></span>

* <span data-ttu-id="6695f-185">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6695f-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="6695f-186">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6695f-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="6695f-187">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="6695f-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="6695f-188">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="6695f-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="6695f-189">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="6695f-190">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-190">July 28, 2017</span></span>

<span data-ttu-id="6695f-191">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="6695f-191">Version 2.0.12</span></span>

* <span data-ttu-id="6695f-192">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-192">Added container commands</span></span>
* <span data-ttu-id="6695f-193">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-193">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="6695f-194">Core</span><span class="sxs-lookup"><span data-stu-id="6695f-194">Core</span></span>

* <span data-ttu-id="6695f-195">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="6695f-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="6695f-196">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="6695f-197">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="6695f-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="6695f-198">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="6695f-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="6695f-199">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="6695f-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="6695f-200">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="6695f-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="6695f-201">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6695f-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6695f-202">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="6695f-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="6695f-203">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="6695f-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="6695f-204">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="6695f-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="6695f-205">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="6695f-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="6695f-206">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="6695f-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="6695f-207">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6695f-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="6695f-208">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6695f-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="6695f-209">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6695f-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="6695f-210">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="6695f-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="6695f-211">ACR</span><span class="sxs-lookup"><span data-stu-id="6695f-211">ACR</span></span>

* <span data-ttu-id="6695f-212">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="6695f-213">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="6695f-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="6695f-214">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="6695f-215">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="6695f-216">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="6695f-217">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="6695f-218">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-218">ACS</span></span>

* <span data-ttu-id="6695f-219">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="6695f-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="6695f-220">AppService</span><span class="sxs-lookup"><span data-stu-id="6695f-220">Appservice</span></span>

* <span data-ttu-id="6695f-221">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="6695f-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="6695f-222">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="6695f-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="6695f-223">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="6695f-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="6695f-224">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="6695f-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="6695f-225">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="6695f-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="6695f-226">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="6695f-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="6695f-227">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="6695f-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="6695f-228">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="6695f-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="6695f-229">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="6695f-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="6695f-230">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="6695f-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="6695f-231">Batch</span><span class="sxs-lookup"><span data-stu-id="6695f-231">Batch</span></span>

* <span data-ttu-id="6695f-232">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6695f-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="6695f-233">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="6695f-234">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="6695f-235">CDN</span><span class="sxs-lookup"><span data-stu-id="6695f-235">CDN</span></span>

* <span data-ttu-id="6695f-236">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6695f-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="6695f-237">Cloud</span><span class="sxs-lookup"><span data-stu-id="6695f-237">Cloud</span></span>

* <span data-ttu-id="6695f-238">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="6695f-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="6695f-239">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="6695f-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="6695f-240">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="6695f-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="6695f-241">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="6695f-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="6695f-242">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6695f-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6695f-243">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6695f-243">CosmosDB</span></span>

* <span data-ttu-id="6695f-244">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="6695f-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="6695f-245">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6695f-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6695f-246">Data Lake Analytics</span></span>

* <span data-ttu-id="6695f-247">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="6695f-248">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="6695f-249">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6695f-250">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-250">Data Lake Store</span></span>

* <span data-ttu-id="6695f-251">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="6695f-252">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6695f-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="6695f-253">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6695f-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="6695f-254">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6695f-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="6695f-255">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="6695f-255">Interactive</span></span>

* <span data-ttu-id="6695f-256">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="6695f-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="6695f-257">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="6695f-257">Increased test coverage</span></span>
* <span data-ttu-id="6695f-258">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="6695f-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="6695f-259">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="6695f-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="6695f-260">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="6695f-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="6695f-261">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="6695f-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="6695f-262">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6695f-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6695f-263">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-263">Added `--progress` flag</span></span>
* <span data-ttu-id="6695f-264">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="6695f-265">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="6695f-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="6695f-266">IoT</span><span class="sxs-lookup"><span data-stu-id="6695f-266">IoT</span></span>

* <span data-ttu-id="6695f-267">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6695f-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="6695f-268">(3934)</span><span class="sxs-lookup"><span data-stu-id="6695f-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="6695f-269">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="6695f-269">Key vault</span></span>

* <span data-ttu-id="6695f-270">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6695f-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="6695f-271">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6695f-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="6695f-272">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6695f-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6695f-273">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6695f-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6695f-274">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6695f-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="6695f-275">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="6695f-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="6695f-276">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6695f-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="6695f-277">(3307)</span><span class="sxs-lookup"><span data-stu-id="6695f-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="6695f-278">Labor</span><span class="sxs-lookup"><span data-stu-id="6695f-278">Lab</span></span>

* <span data-ttu-id="6695f-279">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="6695f-280">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="6695f-281">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6695f-281">Monitor</span></span>

* <span data-ttu-id="6695f-282">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="6695f-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="6695f-283">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="6695f-284">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="6695f-285">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="6695f-286">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6695f-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="6695f-287">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="6695f-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="6695f-288">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="6695f-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="6695f-289">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="6695f-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="6695f-290">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="6695f-290">`location` no longer required</span></span>
  * <span data-ttu-id="6695f-291">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="6695f-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="6695f-292">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="6695f-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="6695f-293">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="6695f-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="6695f-294">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6695f-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="6695f-295">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="6695f-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="6695f-296">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="6695f-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="6695f-297">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="6695f-298">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6695f-298">Network</span></span>

* <span data-ttu-id="6695f-299">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="6695f-300">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="6695f-301">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6695f-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="6695f-302">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6695f-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="6695f-303">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6695f-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="6695f-304">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="6695f-305">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="6695f-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="6695f-306">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="6695f-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="6695f-307">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="6695f-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="6695f-308">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="6695f-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="6695f-309">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="6695f-310">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="6695f-311">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="6695f-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="6695f-312">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="6695f-313">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="6695f-314">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="6695f-315">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="6695f-316">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="6695f-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="6695f-317">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="6695f-318">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6695f-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="6695f-319">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="6695f-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="6695f-320">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6695f-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="6695f-321">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="6695f-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="6695f-322">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6695f-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="6695f-323">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6695f-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="6695f-324">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6695f-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="6695f-325">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6695f-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="6695f-326">Profil</span><span class="sxs-lookup"><span data-stu-id="6695f-326">Profile</span></span>

* <span data-ttu-id="6695f-327">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="6695f-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="6695f-328">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="6695f-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="6695f-329">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="6695f-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="6695f-330">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="6695f-331">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="6695f-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="6695f-332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6695f-332">RDBMS</span></span>

* <span data-ttu-id="6695f-333">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="6695f-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="6695f-334">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="6695f-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="6695f-335">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="6695f-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="6695f-336">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="6695f-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="6695f-337">Ressource</span><span class="sxs-lookup"><span data-stu-id="6695f-337">Resource</span></span>

* <span data-ttu-id="6695f-338">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6695f-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="6695f-339">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="6695f-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="6695f-340">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="6695f-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="6695f-341">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="6695f-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="6695f-342">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="6695f-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="6695f-343">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="6695f-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="6695f-344">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="6695f-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="6695f-345">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="6695f-346">Rolle</span><span class="sxs-lookup"><span data-stu-id="6695f-346">Role</span></span>

* <span data-ttu-id="6695f-347">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6695f-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="6695f-348">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="6695f-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="6695f-349">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="6695f-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="6695f-350">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="6695f-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="6695f-351">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6695f-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6695f-352">Service Fabric</span></span>
* <span data-ttu-id="6695f-353">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="6695f-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="6695f-354">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="6695f-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="6695f-355">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="6695f-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="6695f-356">SQL</span><span class="sxs-lookup"><span data-stu-id="6695f-356">SQL</span></span>

* <span data-ttu-id="6695f-357">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="6695f-358">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6695f-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="6695f-359">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="6695f-360">Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-360">Storage</span></span>

* <span data-ttu-id="6695f-361">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="6695f-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="6695f-362">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6695f-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="6695f-363">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="6695f-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="6695f-364">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="6695f-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="6695f-365">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="6695f-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="6695f-366">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="6695f-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="6695f-367">VM</span><span class="sxs-lookup"><span data-stu-id="6695f-367">VM</span></span>

* <span data-ttu-id="6695f-368">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="6695f-368">Support configuring nsg</span></span>
* <span data-ttu-id="6695f-369">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="6695f-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="6695f-370">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="6695f-370">Support managed service identities</span></span>
* <span data-ttu-id="6695f-371">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="6695f-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="6695f-372">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="6695f-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="6695f-373">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-373">May 10, 2017</span></span>

<span data-ttu-id="6695f-374">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="6695f-374">Version 2.0.6</span></span>

* <span data-ttu-id="6695f-375">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="6695f-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="6695f-376">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="6695f-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="6695f-377">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="6695f-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="6695f-378">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="6695f-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="6695f-379">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="6695f-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="6695f-380">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="6695f-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="6695f-381">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="6695f-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="6695f-382">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="6695f-382">Remove Container module.</span></span>
* <span data-ttu-id="6695f-383">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="6695f-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="6695f-384">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6695f-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="6695f-385">Core</span><span class="sxs-lookup"><span data-stu-id="6695f-385">Core</span></span>

* <span data-ttu-id="6695f-386">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="6695f-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="6695f-387">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="6695f-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="6695f-388">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="6695f-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="6695f-389">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="6695f-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="6695f-390">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="6695f-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="6695f-391">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="6695f-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="6695f-392">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="6695f-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="6695f-393">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="6695f-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="6695f-394">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="6695f-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="6695f-395">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="6695f-395">core: Improved performance</span></span>
* <span data-ttu-id="6695f-396">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="6695f-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="6695f-397">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="6695f-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="6695f-398">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-398">ACS</span></span>

* <span data-ttu-id="6695f-399">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6695f-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="6695f-400">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="6695f-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="6695f-401">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="6695f-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="6695f-402">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="6695f-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="6695f-403">AppService</span><span class="sxs-lookup"><span data-stu-id="6695f-403">AppService</span></span>

* <span data-ttu-id="6695f-404">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="6695f-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="6695f-405">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="6695f-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="6695f-406">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="6695f-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="6695f-407">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="6695f-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="6695f-408">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="6695f-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="6695f-409">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="6695f-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="6695f-410">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="6695f-410">support slot swap with preview</span></span>
* <span data-ttu-id="6695f-411">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="6695f-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="6695f-412">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="6695f-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6695f-413">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6695f-413">CosmosDB</span></span>

* <span data-ttu-id="6695f-414">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="6695f-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="6695f-415">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="6695f-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="6695f-416">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="6695f-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="6695f-417">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="6695f-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6695f-418">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6695f-418">Data Lake Analytics</span></span>

* <span data-ttu-id="6695f-419">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="6695f-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="6695f-420">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="6695f-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="6695f-421">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="6695f-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="6695f-422">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="6695f-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="6695f-423">Table</span><span class="sxs-lookup"><span data-stu-id="6695f-423">Table</span></span>
  * <span data-ttu-id="6695f-424">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="6695f-424">Table valued function</span></span>
  * <span data-ttu-id="6695f-425">Sicht</span><span class="sxs-lookup"><span data-stu-id="6695f-425">View</span></span>
  * <span data-ttu-id="6695f-426">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="6695f-426">Table Statistics.</span></span> <span data-ttu-id="6695f-427">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="6695f-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6695f-428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6695f-428">Data Lake Store</span></span>

* <span data-ttu-id="6695f-429">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="6695f-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="6695f-430">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6695f-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="6695f-431">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="6695f-431">missed help for access show.</span></span> <span data-ttu-id="6695f-432">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6695f-432">adding it.</span></span> <span data-ttu-id="6695f-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="6695f-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="6695f-434">Suchen</span><span class="sxs-lookup"><span data-stu-id="6695f-434">Find</span></span>

* <span data-ttu-id="6695f-435">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="6695f-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="6695f-436">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6695f-436">KeyVault</span></span>

* <span data-ttu-id="6695f-437">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="6695f-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="6695f-438">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="6695f-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="6695f-439">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="6695f-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="6695f-440">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="6695f-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="6695f-441">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="6695f-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="6695f-442">Labor</span><span class="sxs-lookup"><span data-stu-id="6695f-442">Lab</span></span>

* <span data-ttu-id="6695f-443">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="6695f-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="6695f-444">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="6695f-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="6695f-445">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="6695f-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="6695f-446">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="6695f-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="6695f-447">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="6695f-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="6695f-448">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6695f-448">Monitor</span></span>

* <span data-ttu-id="6695f-449">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="6695f-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="6695f-450">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="6695f-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="6695f-451">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6695f-451">Network</span></span>

* <span data-ttu-id="6695f-452">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="6695f-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="6695f-453">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="6695f-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="6695f-454">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="6695f-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="6695f-455">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="6695f-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="6695f-456">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="6695f-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="6695f-457">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="6695f-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="6695f-458">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6695f-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="6695f-459">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6695f-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="6695f-460">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="6695f-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="6695f-461">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="6695f-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="6695f-462">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="6695f-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="6695f-463">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="6695f-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="6695f-464">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="6695f-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="6695f-465">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6695f-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="6695f-466">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6695f-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="6695f-467">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="6695f-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="6695f-468">Profil</span><span class="sxs-lookup"><span data-stu-id="6695f-468">Profile</span></span>

* <span data-ttu-id="6695f-469">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="6695f-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="6695f-470">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="6695f-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="6695f-471">Redis</span><span class="sxs-lookup"><span data-stu-id="6695f-471">Redis</span></span>

* <span data-ttu-id="6695f-472">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="6695f-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="6695f-473">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="6695f-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="6695f-474">Ressource</span><span class="sxs-lookup"><span data-stu-id="6695f-474">Resource</span></span>

* <span data-ttu-id="6695f-475">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="6695f-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="6695f-476">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="6695f-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="6695f-477">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="6695f-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="6695f-478">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="6695f-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="6695f-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="6695f-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="6695f-480">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="6695f-480">Add docs for az lock update.</span></span> <span data-ttu-id="6695f-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="6695f-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="6695f-482">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="6695f-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="6695f-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="6695f-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="6695f-484">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="6695f-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="6695f-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="6695f-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="6695f-486">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="6695f-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="6695f-487">Rolle</span><span class="sxs-lookup"><span data-stu-id="6695f-487">Role</span></span>

* <span data-ttu-id="6695f-488">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="6695f-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="6695f-489">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="6695f-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="6695f-490">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="6695f-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="6695f-491">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="6695f-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="6695f-492">SQL</span><span class="sxs-lookup"><span data-stu-id="6695f-492">SQL</span></span>

* <span data-ttu-id="6695f-493">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="6695f-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="6695f-494">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="6695f-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="6695f-495">Speicher</span><span class="sxs-lookup"><span data-stu-id="6695f-495">Storage</span></span>

* <span data-ttu-id="6695f-496">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="6695f-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="6695f-497">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="6695f-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="6695f-498">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="6695f-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="6695f-499">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="6695f-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="6695f-500">VM</span><span class="sxs-lookup"><span data-stu-id="6695f-500">VM</span></span>

* <span data-ttu-id="6695f-501">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="6695f-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="6695f-502">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="6695f-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="6695f-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="6695f-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="6695f-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="6695f-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="6695f-505">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="6695f-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="6695f-506">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="6695f-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="6695f-507">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="6695f-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="6695f-508">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-508">April 3, 2017</span></span>

<span data-ttu-id="6695f-509">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="6695f-509">Version 2.0.2</span></span>

<span data-ttu-id="6695f-510">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="6695f-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="6695f-511">Core</span><span class="sxs-lookup"><span data-stu-id="6695f-511">Core</span></span>

* <span data-ttu-id="6695f-512">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="6695f-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="6695f-513">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="6695f-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="6695f-514">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="6695f-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="6695f-515">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6695f-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6695f-516">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="6695f-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="6695f-517">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="6695f-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="6695f-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="6695f-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="6695f-519">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="6695f-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="6695f-520">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="6695f-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="6695f-521">ACS</span><span class="sxs-lookup"><span data-stu-id="6695f-521">ACS</span></span>

* <span data-ttu-id="6695f-522">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="6695f-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="6695f-523">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="6695f-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="6695f-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="6695f-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="6695f-525">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="6695f-525">Add support for windows clusters.</span></span> <span data-ttu-id="6695f-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="6695f-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="6695f-527">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="6695f-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="6695f-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="6695f-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="6695f-529">AppService</span><span class="sxs-lookup"><span data-stu-id="6695f-529">AppService</span></span>

* <span data-ttu-id="6695f-530">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="6695f-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="6695f-531">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="6695f-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="6695f-532">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="6695f-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="6695f-533">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="6695f-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="6695f-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="6695f-534">DataLake</span></span>

* <span data-ttu-id="6695f-535">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="6695f-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="6695f-536">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="6695f-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="6695f-537">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="6695f-537">DocuemntDB</span></span>

* <span data-ttu-id="6695f-538">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="6695f-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="6695f-539">VM</span><span class="sxs-lookup"><span data-stu-id="6695f-539">VM</span></span>

* <span data-ttu-id="6695f-540">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="6695f-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="6695f-541">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="6695f-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="6695f-542">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="6695f-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="6695f-543">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6695f-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6695f-544">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="6695f-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="6695f-545">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="6695f-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="6695f-546">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="6695f-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="6695f-547">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="6695f-547">February 27, 2017</span></span>

<span data-ttu-id="6695f-548">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="6695f-548">Version 2.0.0</span></span>

<span data-ttu-id="6695f-549">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="6695f-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="6695f-550">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="6695f-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="6695f-551">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="6695f-551">Container Service (acs)</span></span>
- <span data-ttu-id="6695f-552">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="6695f-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="6695f-553">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6695f-553">Networking</span></span>
- <span data-ttu-id="6695f-554">Storage</span><span class="sxs-lookup"><span data-stu-id="6695f-554">Storage</span></span>

<span data-ttu-id="6695f-555">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6695f-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="6695f-556">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="6695f-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="6695f-557">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="6695f-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="6695f-558">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="6695f-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="6695f-559">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="6695f-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="6695f-560">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="6695f-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="6695f-561">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="6695f-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="6695f-562">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="6695f-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="6695f-563">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="6695f-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="6695f-564">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="6695f-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="6695f-565">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="6695f-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="6695f-566">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="6695f-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="6695f-567">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="6695f-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="6695f-568">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="6695f-568">Provide feedback from the command line with the `az feedback` command.</span></span>

