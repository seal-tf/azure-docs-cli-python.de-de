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
ms.openlocfilehash: 761bd61474e7c72fb2daeb756828f00196b56c3a
ms.sourcegitcommit: bb649ebd7e7fce8fb5008ac1e2e2c33481a45df9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/16/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="67fed-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="67fed-104">Azure CLI 2.0 release notes</span></span>

## <a name="november-14-2017"></a><span data-ttu-id="67fed-105">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-105">November 14, 2017</span></span>

<span data-ttu-id="67fed-106">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="67fed-106">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="67fed-107">ACR</span><span class="sxs-lookup"><span data-stu-id="67fed-107">ACR</span></span>

* <span data-ttu-id="67fed-108">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-108">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="67fed-109">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-109">ACS</span></span>

* <span data-ttu-id="67fed-110">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="67fed-110">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="67fed-111">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="67fed-111">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="67fed-112">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="67fed-112">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="67fed-113">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-113">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="67fed-114">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-114">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-115">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-115">Appservice</span></span>

* <span data-ttu-id="67fed-116">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-116">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="67fed-117">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-117">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="67fed-118">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-118">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="67fed-119">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-119">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="67fed-120">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-120">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="67fed-121">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="67fed-121">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="67fed-122">Batch</span><span class="sxs-lookup"><span data-stu-id="67fed-122">Batch</span></span>

* <span data-ttu-id="67fed-123">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="67fed-123">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="67fed-124">BatchAI</span><span class="sxs-lookup"><span data-stu-id="67fed-124">Batchai</span></span>

* <span data-ttu-id="67fed-125">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-125">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="67fed-126">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-126">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="67fed-127">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-127">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="67fed-128">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-128">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="67fed-129">Cloud</span><span class="sxs-lookup"><span data-stu-id="67fed-129">Cloud</span></span>

* <span data-ttu-id="67fed-130">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="67fed-130">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="67fed-131">Container</span><span class="sxs-lookup"><span data-stu-id="67fed-131">Container</span></span>

* <span data-ttu-id="67fed-132">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-132">Added support to open multiple ports</span></span>
* <span data-ttu-id="67fed-133">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-133">Added container group restart policy</span></span>
* <span data-ttu-id="67fed-134">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-134">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="67fed-135">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67fed-135">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67fed-136">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67fed-136">Data Lake Analytics</span></span>

* <span data-ttu-id="67fed-137">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="67fed-137">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67fed-138">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-138">Data Lake Store</span></span>

* <span data-ttu-id="67fed-139">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="67fed-139">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="67fed-140">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67fed-140">Extension</span></span>

* <span data-ttu-id="67fed-141">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67fed-141">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="67fed-142">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="67fed-142">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="67fed-143">IoT</span><span class="sxs-lookup"><span data-stu-id="67fed-143">IoT</span></span>

* <span data-ttu-id="67fed-144">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-144">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="67fed-145">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67fed-145">Monitor</span></span>

* <span data-ttu-id="67fed-146">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-146">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="67fed-147">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-147">Network</span></span>

* <span data-ttu-id="67fed-148">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-148">Added support for CAA DNS records</span></span>
* <span data-ttu-id="67fed-149">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="67fed-149">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="67fed-150">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="67fed-150">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="67fed-151">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-151">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="67fed-152">Reservations</span><span class="sxs-lookup"><span data-stu-id="67fed-152">Reservations</span></span>

* <span data-ttu-id="67fed-153">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67fed-153">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-154">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-154">Resource</span></span>

* <span data-ttu-id="67fed-155">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-155">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-156">SQL</span><span class="sxs-lookup"><span data-stu-id="67fed-156">SQL</span></span>

* <span data-ttu-id="67fed-157">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-157">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-158">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-158">Storage</span></span>

* <span data-ttu-id="67fed-159">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="67fed-159">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="67fed-160">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="67fed-160">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="67fed-161">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="67fed-161">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="67fed-162">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-162">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="67fed-163">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-163">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="67fed-164">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-164">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="67fed-165">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-165">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-166">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-166">VM</span></span>

* <span data-ttu-id="67fed-167">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="67fed-167">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="67fed-168">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-168">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="67fed-169">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="67fed-169">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="67fed-170">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-170">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="67fed-171">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-171">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="67fed-172">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-172">October 24, 2017</span></span>

<span data-ttu-id="67fed-173">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="67fed-173">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="67fed-174">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-174">Core</span></span>

* <span data-ttu-id="67fed-175">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="67fed-175">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="67fed-176">ACR</span><span class="sxs-lookup"><span data-stu-id="67fed-176">ACR</span></span>

* <span data-ttu-id="67fed-177">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="67fed-177">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="67fed-178">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="67fed-178">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="67fed-179">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="67fed-179">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-180">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-180">ACS</span></span>

* <span data-ttu-id="67fed-181">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-181">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="67fed-182">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-182">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-183">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-183">Appservice</span></span>

* <span data-ttu-id="67fed-184">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="67fed-184">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="67fed-185">Komponente</span><span class="sxs-lookup"><span data-stu-id="67fed-185">Component</span></span>

* <span data-ttu-id="67fed-186">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-186">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="67fed-187">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67fed-187">Monitor</span></span>

* <span data-ttu-id="67fed-188">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-188">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-189">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-189">Resource</span></span>

* <span data-ttu-id="67fed-190">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-190">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="67fed-191">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="67fed-191">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-192">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-192">VM</span></span>

* <span data-ttu-id="67fed-193">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-193">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="67fed-194">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-194">October 9, 2017</span></span>

<span data-ttu-id="67fed-195">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="67fed-195">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="67fed-196">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-196">Core</span></span>

* <span data-ttu-id="67fed-197">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67fed-197">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-198">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-198">Appservice</span></span>

* <span data-ttu-id="67fed-199">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67fed-199">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="67fed-200">Batch</span><span class="sxs-lookup"><span data-stu-id="67fed-200">Batch</span></span>

* <span data-ttu-id="67fed-201">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="67fed-201">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="67fed-202">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="67fed-202">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="67fed-203">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-203">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="67fed-204">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-204">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="67fed-205">BatchAI</span><span class="sxs-lookup"><span data-stu-id="67fed-205">Batchai</span></span>

* <span data-ttu-id="67fed-206">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="67fed-206">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="67fed-207">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67fed-207">Keyvault</span></span>

* <span data-ttu-id="67fed-208">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="67fed-208">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="67fed-209">(#4448)</span><span class="sxs-lookup"><span data-stu-id="67fed-209">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="67fed-210">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-210">Network</span></span>

* <span data-ttu-id="67fed-211">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="67fed-211">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="67fed-212">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="67fed-212">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-213">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-213">Resource</span></span>

* <span data-ttu-id="67fed-214">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-214">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="67fed-215">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67fed-215">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="67fed-216">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67fed-216">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="67fed-217">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67fed-217">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-218">Sql</span><span class="sxs-lookup"><span data-stu-id="67fed-218">Sql</span></span>

* <span data-ttu-id="67fed-219">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-219">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="67fed-220">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67fed-220">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="67fed-221">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="67fed-221">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-222">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-222">Storage</span></span>

* <span data-ttu-id="67fed-223">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-223">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-224">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-224">Vm</span></span>

* <span data-ttu-id="67fed-225">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="67fed-225">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="67fed-226">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-226">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="67fed-227">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-227">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="67fed-228">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-228">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="67fed-229">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-229">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="67fed-230">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-230">September 22, 2017</span></span>

<span data-ttu-id="67fed-231">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="67fed-231">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-232">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-232">Resource</span></span>

* <span data-ttu-id="67fed-233">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-233">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="67fed-234">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-234">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="67fed-235">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-235">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="67fed-236">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="67fed-236">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="67fed-237">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-237">Network</span></span>

* <span data-ttu-id="67fed-238">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-238">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="67fed-239">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-239">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="67fed-240">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-240">Added `asg` application security group commands</span></span>
* <span data-ttu-id="67fed-241">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-241">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="67fed-242">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-242">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="67fed-243">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-243">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="67fed-244">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-244">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-245">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-245">Storage</span></span>

* <span data-ttu-id="67fed-246">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67fed-246">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="67fed-247">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="67fed-247">Eventgrid</span></span>

* <span data-ttu-id="67fed-248">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67fed-248">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-249">SQL</span><span class="sxs-lookup"><span data-stu-id="67fed-249">SQL</span></span>

* <span data-ttu-id="67fed-250">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="67fed-250">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="67fed-251">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67fed-251">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="67fed-252">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-252">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="67fed-253">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67fed-253">Keyvault</span></span>

* <span data-ttu-id="67fed-254">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-254">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-255">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-255">VM</span></span>

* <span data-ttu-id="67fed-256">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-256">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="67fed-257">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67fed-257">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="67fed-258">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-258">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="67fed-259">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-259">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="67fed-260">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-260">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="67fed-261">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-261">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-262">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-262">ACS</span></span>

* <span data-ttu-id="67fed-263">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-263">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-264">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-264">Appservice</span></span>

* <span data-ttu-id="67fed-265">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="67fed-265">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="67fed-266">Backup </span><span class="sxs-lookup"><span data-stu-id="67fed-266">Backup</span></span>

* <span data-ttu-id="67fed-267">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67fed-267">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="67fed-268">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-268">September 11, 2017</span></span>

<span data-ttu-id="67fed-269">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="67fed-269">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="67fed-270">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-270">Core</span></span>

* <span data-ttu-id="67fed-271">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="67fed-271">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="67fed-272">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="67fed-272">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-273">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-273">Acs</span></span>

* <span data-ttu-id="67fed-274">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-274">Added `acs list-locations` command</span></span>
* <span data-ttu-id="67fed-275">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="67fed-275">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-276">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-276">Appservice</span></span>

* <span data-ttu-id="67fed-277">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="67fed-277">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="67fed-278">CDN</span><span class="sxs-lookup"><span data-stu-id="67fed-278">CDN</span></span>

* <span data-ttu-id="67fed-279">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="67fed-279">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="67fed-280">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="67fed-280">Extension</span></span>

* <span data-ttu-id="67fed-281">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="67fed-281">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="67fed-282">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67fed-282">Keyvault</span></span>

* <span data-ttu-id="67fed-283">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="67fed-283">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="67fed-284">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-284">Network</span></span>

* <span data-ttu-id="67fed-285">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-285">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="67fed-286">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="67fed-286">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="67fed-287">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-287">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="67fed-288">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-288">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="67fed-289">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-289">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-290">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-290">Resource</span></span>

* <span data-ttu-id="67fed-291">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="67fed-291">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="67fed-292">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="67fed-292">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="67fed-293">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="67fed-293">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="67fed-294">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="67fed-294">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-295">SQL</span><span class="sxs-lookup"><span data-stu-id="67fed-295">SQL</span></span>

* <span data-ttu-id="67fed-296">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-296">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-297">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-297">VM</span></span>

* <span data-ttu-id="67fed-298">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="67fed-298">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="67fed-299">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="67fed-299">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="67fed-300">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-300">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="67fed-301">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="67fed-301">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="67fed-302">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="67fed-302">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="67fed-303">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-303">August 31, 2017</span></span>

<span data-ttu-id="67fed-304">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="67fed-304">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="67fed-305">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67fed-305">Keyvault</span></span>

* <span data-ttu-id="67fed-306">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="67fed-306">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="67fed-307">Sf</span><span class="sxs-lookup"><span data-stu-id="67fed-307">Sf</span></span>

* <span data-ttu-id="67fed-308">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="67fed-308">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-309">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-309">Storage</span></span>

* <span data-ttu-id="67fed-310">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="67fed-310">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="67fed-311">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="67fed-311">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="67fed-312">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-312">August 28, 2017</span></span>

<span data-ttu-id="67fed-313">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="67fed-313">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="67fed-314">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="67fed-314">CLI</span></span>

* <span data-ttu-id="67fed-315">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67fed-315">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-316">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-316">ACS</span></span>

* <span data-ttu-id="67fed-317">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="67fed-317">Corrected preview regions.</span></span>
* <span data-ttu-id="67fed-318">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="67fed-318">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="67fed-319">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="67fed-319">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-320">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-320">Appservice</span></span>

* <span data-ttu-id="67fed-321">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-321">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="67fed-322">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-322">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="67fed-323">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67fed-323">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="67fed-324">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="67fed-324">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="67fed-325">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="67fed-325">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="67fed-326">IoT</span><span class="sxs-lookup"><span data-stu-id="67fed-326">IoT</span></span>

* <span data-ttu-id="67fed-327">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="67fed-327">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="67fed-328">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-328">Network</span></span>

* <span data-ttu-id="67fed-329">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-329">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="67fed-330">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-330">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="67fed-331">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-331">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="67fed-332">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-332">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="67fed-333">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-333">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="67fed-334">Profil</span><span class="sxs-lookup"><span data-stu-id="67fed-334">Profile</span></span>

* <span data-ttu-id="67fed-335">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67fed-335">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="67fed-336">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67fed-336">Service Fabric</span></span>

* <span data-ttu-id="67fed-337">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="67fed-337">Preview release</span></span>
* <span data-ttu-id="67fed-338">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="67fed-338">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="67fed-339">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-339">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="67fed-340">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-340">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-341">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-341">Storage</span></span>

* <span data-ttu-id="67fed-342">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67fed-342">Enabled setting blob tier</span></span>
* <span data-ttu-id="67fed-343">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-343">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="67fed-344">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-344">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="67fed-345">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67fed-345">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="67fed-346">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-346">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="67fed-347">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="67fed-347">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-348">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-348">VM</span></span>

* <span data-ttu-id="67fed-349">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-349">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="67fed-350">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="67fed-350">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="67fed-351">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-351">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="67fed-352">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="67fed-352">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="67fed-353">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-353">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="67fed-354">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="67fed-354">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="67fed-355">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-355">August 15, 2017</span></span>

<span data-ttu-id="67fed-356">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="67fed-356">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-357">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-357">ACS</span></span>

* <span data-ttu-id="67fed-358">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-358">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-359">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-359">Appservice</span></span>

* <span data-ttu-id="67fed-360">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-360">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="67fed-361">Event Grid</span><span class="sxs-lookup"><span data-stu-id="67fed-361">Event Grid</span></span>

* <span data-ttu-id="67fed-362">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-362">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="67fed-363">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-363">August 11, 2017</span></span>

<span data-ttu-id="67fed-364">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="67fed-364">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-365">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-365">ACS</span></span>

* <span data-ttu-id="67fed-366">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-366">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="67fed-367">Batch</span><span class="sxs-lookup"><span data-stu-id="67fed-367">Batch</span></span>

* <span data-ttu-id="67fed-368">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67fed-368">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="67fed-369">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-369">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="67fed-370">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-370">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="67fed-371">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="67fed-371">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="67fed-372">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="67fed-372">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="67fed-373">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-373">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="67fed-374">Komponente</span><span class="sxs-lookup"><span data-stu-id="67fed-374">Component</span></span>

* <span data-ttu-id="67fed-375">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-375">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="67fed-376">Container</span><span class="sxs-lookup"><span data-stu-id="67fed-376">Container</span></span>

* <span data-ttu-id="67fed-377">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="67fed-377">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="67fed-378">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-378">Data Lake Store</span></span>

* <span data-ttu-id="67fed-379">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67fed-379">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="67fed-380">Event Grid</span><span class="sxs-lookup"><span data-stu-id="67fed-380">Event Grid</span></span>

* <span data-ttu-id="67fed-381">Erste Version</span><span class="sxs-lookup"><span data-stu-id="67fed-381">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="67fed-382">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-382">Network</span></span>

* <span data-ttu-id="67fed-383">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-383">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="67fed-384">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="67fed-384">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="67fed-385">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="67fed-385">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="67fed-386">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="67fed-386">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="67fed-387">Profil</span><span class="sxs-lookup"><span data-stu-id="67fed-387">Profile</span></span>

* <span data-ttu-id="67fed-388">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="67fed-388">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-389">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-389">Storage</span></span>

* <span data-ttu-id="67fed-390">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67fed-390">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-391">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-391">VM</span></span>

* <span data-ttu-id="67fed-392">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67fed-392">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="67fed-393">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67fed-393">Exposed `list-skus` command</span></span>
* <span data-ttu-id="67fed-394">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="67fed-394">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="67fed-395">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="67fed-395">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="67fed-396">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-396">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="67fed-397">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-397">July 28, 2017</span></span>

<span data-ttu-id="67fed-398">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="67fed-398">Version 2.0.12</span></span>

* <span data-ttu-id="67fed-399">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-399">Added container commands</span></span>
* <span data-ttu-id="67fed-400">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-400">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="67fed-401">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-401">Core</span></span>

* <span data-ttu-id="67fed-402">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="67fed-402">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="67fed-403">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-403">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="67fed-404">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="67fed-404">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="67fed-405">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="67fed-405">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="67fed-406">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="67fed-406">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="67fed-407">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="67fed-407">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="67fed-408">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="67fed-408">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="67fed-409">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="67fed-409">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="67fed-410">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="67fed-410">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="67fed-411">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="67fed-411">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="67fed-412">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="67fed-412">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="67fed-413">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="67fed-413">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="67fed-414">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="67fed-414">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="67fed-415">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="67fed-415">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="67fed-416">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="67fed-416">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="67fed-417">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="67fed-417">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="67fed-418">ACR</span><span class="sxs-lookup"><span data-stu-id="67fed-418">ACR</span></span>

* <span data-ttu-id="67fed-419">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-419">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="67fed-420">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="67fed-420">Support SKU update for managed registries</span></span>
* <span data-ttu-id="67fed-421">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-421">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="67fed-422">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-422">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="67fed-423">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-423">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="67fed-424">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-424">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-425">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-425">ACS</span></span>

* <span data-ttu-id="67fed-426">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="67fed-426">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-427">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-427">Appservice</span></span>

* <span data-ttu-id="67fed-428">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="67fed-428">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="67fed-429">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="67fed-429">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="67fed-430">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="67fed-430">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="67fed-431">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="67fed-431">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="67fed-432">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="67fed-432">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="67fed-433">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="67fed-433">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="67fed-434">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="67fed-434">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="67fed-435">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="67fed-435">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="67fed-436">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="67fed-436">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="67fed-437">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="67fed-437">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="67fed-438">Batch</span><span class="sxs-lookup"><span data-stu-id="67fed-438">Batch</span></span>

* <span data-ttu-id="67fed-439">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67fed-439">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="67fed-440">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-440">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="67fed-441">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-441">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="67fed-442">CDN</span><span class="sxs-lookup"><span data-stu-id="67fed-442">CDN</span></span>

* <span data-ttu-id="67fed-443">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="67fed-443">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="67fed-444">Cloud</span><span class="sxs-lookup"><span data-stu-id="67fed-444">Cloud</span></span>

* <span data-ttu-id="67fed-445">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="67fed-445">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="67fed-446">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="67fed-446">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="67fed-447">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="67fed-447">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="67fed-448">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="67fed-448">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="67fed-449">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="67fed-449">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67fed-450">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67fed-450">CosmosDB</span></span>

* <span data-ttu-id="67fed-451">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="67fed-451">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="67fed-452">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-452">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67fed-453">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67fed-453">Data Lake Analytics</span></span>

* <span data-ttu-id="67fed-454">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-454">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="67fed-455">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-455">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="67fed-456">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-456">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67fed-457">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-457">Data Lake Store</span></span>

* <span data-ttu-id="67fed-458">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-458">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="67fed-459">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="67fed-459">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="67fed-460">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="67fed-460">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="67fed-461">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="67fed-461">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="67fed-462">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="67fed-462">Interactive</span></span>

* <span data-ttu-id="67fed-463">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-463">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="67fed-464">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-464">Increased test coverage</span></span>
* <span data-ttu-id="67fed-465">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="67fed-465">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="67fed-466">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="67fed-466">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="67fed-467">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="67fed-467">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="67fed-468">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="67fed-468">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="67fed-469">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="67fed-469">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="67fed-470">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-470">Added `--progress` flag</span></span>
* <span data-ttu-id="67fed-471">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-471">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="67fed-472">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="67fed-472">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="67fed-473">IoT</span><span class="sxs-lookup"><span data-stu-id="67fed-473">IoT</span></span>

* <span data-ttu-id="67fed-474">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="67fed-474">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="67fed-475">(3934)</span><span class="sxs-lookup"><span data-stu-id="67fed-475">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="67fed-476">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="67fed-476">Key vault</span></span>

* <span data-ttu-id="67fed-477">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="67fed-477">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="67fed-478">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67fed-478">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="67fed-479">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67fed-479">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="67fed-480">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67fed-480">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="67fed-481">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="67fed-481">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="67fed-482">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="67fed-482">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="67fed-483">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="67fed-483">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="67fed-484">(3307)</span><span class="sxs-lookup"><span data-stu-id="67fed-484">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="67fed-485">Labor</span><span class="sxs-lookup"><span data-stu-id="67fed-485">Lab</span></span>

* <span data-ttu-id="67fed-486">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-486">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="67fed-487">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-487">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="67fed-488">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67fed-488">Monitor</span></span>

* <span data-ttu-id="67fed-489">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="67fed-489">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="67fed-490">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-490">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="67fed-491">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-491">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="67fed-492">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-492">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="67fed-493">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="67fed-493">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="67fed-494">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="67fed-494">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="67fed-495">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="67fed-495">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="67fed-496">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="67fed-496">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="67fed-497">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="67fed-497">`location` no longer required</span></span>
  * <span data-ttu-id="67fed-498">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="67fed-498">Add name and ID support for target</span></span>
  * <span data-ttu-id="67fed-499">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="67fed-499">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="67fed-500">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="67fed-500">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="67fed-501">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="67fed-501">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="67fed-502">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="67fed-502">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="67fed-503">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="67fed-503">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="67fed-504">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-504">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="67fed-505">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-505">Network</span></span>

* <span data-ttu-id="67fed-506">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-506">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="67fed-507">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-507">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="67fed-508">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="67fed-508">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="67fed-509">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="67fed-509">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="67fed-510">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="67fed-510">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="67fed-511">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-511">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="67fed-512">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="67fed-512">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="67fed-513">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="67fed-513">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="67fed-514">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="67fed-514">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="67fed-515">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="67fed-515">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="67fed-516">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-516">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="67fed-517">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-517">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="67fed-518">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="67fed-518">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="67fed-519">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-519">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="67fed-520">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-520">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="67fed-521">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-521">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="67fed-522">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-522">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="67fed-523">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="67fed-523">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="67fed-524">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-524">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="67fed-525">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-525">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="67fed-526">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="67fed-526">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="67fed-527">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="67fed-527">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="67fed-528">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-528">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="67fed-529">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67fed-529">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="67fed-530">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67fed-530">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="67fed-531">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67fed-531">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="67fed-532">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="67fed-532">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="67fed-533">Profil</span><span class="sxs-lookup"><span data-stu-id="67fed-533">Profile</span></span>

* <span data-ttu-id="67fed-534">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="67fed-534">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="67fed-535">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="67fed-535">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="67fed-536">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="67fed-536">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="67fed-537">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-537">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="67fed-538">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="67fed-538">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="67fed-539">RDBMS</span><span class="sxs-lookup"><span data-stu-id="67fed-539">RDBMS</span></span>

* <span data-ttu-id="67fed-540">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="67fed-540">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="67fed-541">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="67fed-541">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="67fed-542">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="67fed-542">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="67fed-543">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="67fed-543">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-544">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-544">Resource</span></span>

* <span data-ttu-id="67fed-545">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-545">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="67fed-546">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="67fed-546">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="67fed-547">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-547">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="67fed-548">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="67fed-548">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="67fed-549">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="67fed-549">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="67fed-550">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="67fed-550">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="67fed-551">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="67fed-551">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="67fed-552">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-552">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="67fed-553">Rolle</span><span class="sxs-lookup"><span data-stu-id="67fed-553">Role</span></span>

* <span data-ttu-id="67fed-554">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="67fed-554">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="67fed-555">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="67fed-555">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="67fed-556">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="67fed-556">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="67fed-557">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="67fed-557">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="67fed-558">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-558">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="67fed-559">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67fed-559">Service Fabric</span></span>
* <span data-ttu-id="67fed-560">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="67fed-560">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="67fed-561">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="67fed-561">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="67fed-562">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="67fed-562">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-563">SQL</span><span class="sxs-lookup"><span data-stu-id="67fed-563">SQL</span></span>

* <span data-ttu-id="67fed-564">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-564">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="67fed-565">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="67fed-565">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="67fed-566">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-566">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-567">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-567">Storage</span></span>

* <span data-ttu-id="67fed-568">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="67fed-568">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="67fed-569">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67fed-569">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="67fed-570">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="67fed-570">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="67fed-571">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="67fed-571">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="67fed-572">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="67fed-572">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="67fed-573">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="67fed-573">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-574">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-574">VM</span></span>

* <span data-ttu-id="67fed-575">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="67fed-575">Support configuring nsg</span></span>
* <span data-ttu-id="67fed-576">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="67fed-576">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="67fed-577">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="67fed-577">Support managed service identities</span></span>
* <span data-ttu-id="67fed-578">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="67fed-578">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="67fed-579">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="67fed-579">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="67fed-580">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-580">May 10, 2017</span></span>

<span data-ttu-id="67fed-581">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="67fed-581">Version 2.0.6</span></span>

* <span data-ttu-id="67fed-582">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="67fed-582">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="67fed-583">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="67fed-583">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="67fed-584">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="67fed-584">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="67fed-585">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="67fed-585">Include Cognitive Services module.</span></span>
* <span data-ttu-id="67fed-586">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="67fed-586">Include Service Fabric module.</span></span>
* <span data-ttu-id="67fed-587">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="67fed-587">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="67fed-588">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="67fed-588">Add support for CDN commands.</span></span>
* <span data-ttu-id="67fed-589">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="67fed-589">Remove Container module.</span></span>
* <span data-ttu-id="67fed-590">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="67fed-590">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="67fed-591">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="67fed-591">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="67fed-592">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-592">Core</span></span>

* <span data-ttu-id="67fed-593">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="67fed-593">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="67fed-594">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="67fed-594">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="67fed-595">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="67fed-595">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="67fed-596">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="67fed-596">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="67fed-597">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="67fed-597">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="67fed-598">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="67fed-598">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="67fed-599">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="67fed-599">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="67fed-600">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="67fed-600">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="67fed-601">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="67fed-601">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="67fed-602">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="67fed-602">core: Improved performance</span></span>
* <span data-ttu-id="67fed-603">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="67fed-603">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="67fed-604">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="67fed-604">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="67fed-605">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-605">ACS</span></span>

* <span data-ttu-id="67fed-606">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67fed-606">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="67fed-607">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="67fed-607">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="67fed-608">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="67fed-608">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="67fed-609">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="67fed-609">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="67fed-610">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-610">AppService</span></span>

* <span data-ttu-id="67fed-611">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="67fed-611">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="67fed-612">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="67fed-612">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="67fed-613">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="67fed-613">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="67fed-614">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="67fed-614">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="67fed-615">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="67fed-615">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="67fed-616">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="67fed-616">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="67fed-617">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="67fed-617">support slot swap with preview</span></span>
* <span data-ttu-id="67fed-618">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="67fed-618">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="67fed-619">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="67fed-619">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="67fed-620">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="67fed-620">CosmosDB</span></span>

* <span data-ttu-id="67fed-621">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="67fed-621">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="67fed-622">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="67fed-622">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="67fed-623">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="67fed-623">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="67fed-624">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="67fed-624">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="67fed-625">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="67fed-625">Data Lake Analytics</span></span>

* <span data-ttu-id="67fed-626">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="67fed-626">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="67fed-627">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="67fed-627">Add support for new catalog item type: package.</span></span> <span data-ttu-id="67fed-628">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="67fed-628">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="67fed-629">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="67fed-629">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="67fed-630">Table</span><span class="sxs-lookup"><span data-stu-id="67fed-630">Table</span></span>
  * <span data-ttu-id="67fed-631">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="67fed-631">Table valued function</span></span>
  * <span data-ttu-id="67fed-632">Sicht</span><span class="sxs-lookup"><span data-stu-id="67fed-632">View</span></span>
  * <span data-ttu-id="67fed-633">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="67fed-633">Table Statistics.</span></span> <span data-ttu-id="67fed-634">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="67fed-634">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="67fed-635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="67fed-635">Data Lake Store</span></span>

* <span data-ttu-id="67fed-636">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="67fed-636">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="67fed-637">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="67fed-637">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="67fed-638">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="67fed-638">missed help for access show.</span></span> <span data-ttu-id="67fed-639">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="67fed-639">adding it.</span></span> <span data-ttu-id="67fed-640">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="67fed-640">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="67fed-641">Suchen</span><span class="sxs-lookup"><span data-stu-id="67fed-641">Find</span></span>

* <span data-ttu-id="67fed-642">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="67fed-642">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="67fed-643">KeyVault</span><span class="sxs-lookup"><span data-stu-id="67fed-643">KeyVault</span></span>

* <span data-ttu-id="67fed-644">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="67fed-644">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="67fed-645">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="67fed-645">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="67fed-646">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="67fed-646">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="67fed-647">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="67fed-647">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="67fed-648">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="67fed-648">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="67fed-649">Labor</span><span class="sxs-lookup"><span data-stu-id="67fed-649">Lab</span></span>

* <span data-ttu-id="67fed-650">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="67fed-650">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="67fed-651">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="67fed-651">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="67fed-652">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="67fed-652">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="67fed-653">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="67fed-653">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="67fed-654">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="67fed-654">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="67fed-655">Überwachen</span><span class="sxs-lookup"><span data-stu-id="67fed-655">Monitor</span></span>

* <span data-ttu-id="67fed-656">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="67fed-656">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="67fed-657">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="67fed-657">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="67fed-658">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-658">Network</span></span>

* <span data-ttu-id="67fed-659">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="67fed-659">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="67fed-660">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="67fed-660">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="67fed-661">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="67fed-661">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="67fed-662">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="67fed-662">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="67fed-663">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="67fed-663">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="67fed-664">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="67fed-664">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="67fed-665">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="67fed-665">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="67fed-666">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="67fed-666">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="67fed-667">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="67fed-667">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="67fed-668">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="67fed-668">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="67fed-669">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="67fed-669">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="67fed-670">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="67fed-670">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="67fed-671">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="67fed-671">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="67fed-672">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="67fed-672">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="67fed-673">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="67fed-673">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="67fed-674">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="67fed-674">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="67fed-675">Profil</span><span class="sxs-lookup"><span data-stu-id="67fed-675">Profile</span></span>

* <span data-ttu-id="67fed-676">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="67fed-676">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="67fed-677">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="67fed-677">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="67fed-678">Redis</span><span class="sxs-lookup"><span data-stu-id="67fed-678">Redis</span></span>

* <span data-ttu-id="67fed-679">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="67fed-679">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="67fed-680">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="67fed-680">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="67fed-681">Ressource</span><span class="sxs-lookup"><span data-stu-id="67fed-681">Resource</span></span>

* <span data-ttu-id="67fed-682">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="67fed-682">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="67fed-683">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="67fed-683">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="67fed-684">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="67fed-684">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="67fed-685">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="67fed-685">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="67fed-686">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="67fed-686">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="67fed-687">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="67fed-687">Add docs for az lock update.</span></span> <span data-ttu-id="67fed-688">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="67fed-688">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="67fed-689">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="67fed-689">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="67fed-690">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="67fed-690">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="67fed-691">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="67fed-691">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="67fed-692">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="67fed-692">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="67fed-693">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="67fed-693">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="67fed-694">Rolle</span><span class="sxs-lookup"><span data-stu-id="67fed-694">Role</span></span>

* <span data-ttu-id="67fed-695">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="67fed-695">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="67fed-696">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="67fed-696">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="67fed-697">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="67fed-697">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="67fed-698">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="67fed-698">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="67fed-699">SQL</span><span class="sxs-lookup"><span data-stu-id="67fed-699">SQL</span></span>

* <span data-ttu-id="67fed-700">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="67fed-700">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="67fed-701">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="67fed-701">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="67fed-702">Speicher</span><span class="sxs-lookup"><span data-stu-id="67fed-702">Storage</span></span>

* <span data-ttu-id="67fed-703">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="67fed-703">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="67fed-704">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="67fed-704">Add support for incremental blob copy</span></span>
* <span data-ttu-id="67fed-705">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="67fed-705">Add support for large block blob upload</span></span>
* <span data-ttu-id="67fed-706">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="67fed-706">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-707">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-707">VM</span></span>

* <span data-ttu-id="67fed-708">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="67fed-708">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="67fed-709">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="67fed-709">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="67fed-710">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="67fed-710">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="67fed-711">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="67fed-711">az vm/vmss disk</span></span>
  3. <span data-ttu-id="67fed-712">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="67fed-712">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="67fed-713">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="67fed-713">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="67fed-714">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="67fed-714">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="67fed-715">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-715">April 3, 2017</span></span>

<span data-ttu-id="67fed-716">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="67fed-716">Version 2.0.2</span></span>

<span data-ttu-id="67fed-717">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="67fed-717">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="67fed-718">Core</span><span class="sxs-lookup"><span data-stu-id="67fed-718">Core</span></span>

* <span data-ttu-id="67fed-719">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="67fed-719">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="67fed-720">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="67fed-720">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="67fed-721">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="67fed-721">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="67fed-722">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="67fed-722">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="67fed-723">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="67fed-723">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="67fed-724">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="67fed-724">Add prompting for missing template parameters.</span></span> <span data-ttu-id="67fed-725">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="67fed-725">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="67fed-726">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="67fed-726">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="67fed-727">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="67fed-727">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="67fed-728">ACS</span><span class="sxs-lookup"><span data-stu-id="67fed-728">ACS</span></span>

* <span data-ttu-id="67fed-729">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="67fed-729">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="67fed-730">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="67fed-730">Add support for ssh key password prompting.</span></span> <span data-ttu-id="67fed-731">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="67fed-731">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="67fed-732">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="67fed-732">Add support for windows clusters.</span></span> <span data-ttu-id="67fed-733">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="67fed-733">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="67fed-734">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="67fed-734">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="67fed-735">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="67fed-735">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="67fed-736">AppService</span><span class="sxs-lookup"><span data-stu-id="67fed-736">AppService</span></span>

* <span data-ttu-id="67fed-737">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="67fed-737">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="67fed-738">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="67fed-738">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="67fed-739">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="67fed-739">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="67fed-740">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="67fed-740">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="67fed-741">DataLake</span><span class="sxs-lookup"><span data-stu-id="67fed-741">DataLake</span></span>

* <span data-ttu-id="67fed-742">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="67fed-742">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="67fed-743">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="67fed-743">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="67fed-744">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="67fed-744">DocuemntDB</span></span>

* <span data-ttu-id="67fed-745">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="67fed-745">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="67fed-746">VM</span><span class="sxs-lookup"><span data-stu-id="67fed-746">VM</span></span>

* <span data-ttu-id="67fed-747">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="67fed-747">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="67fed-748">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="67fed-748">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="67fed-749">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="67fed-749">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="67fed-750">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="67fed-750">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="67fed-751">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="67fed-751">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="67fed-752">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="67fed-752">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="67fed-753">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="67fed-753">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="67fed-754">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="67fed-754">February 27, 2017</span></span>

<span data-ttu-id="67fed-755">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="67fed-755">Version 2.0.0</span></span>

<span data-ttu-id="67fed-756">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="67fed-756">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="67fed-757">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="67fed-757">General availability applies to these command modules:</span></span>
- <span data-ttu-id="67fed-758">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="67fed-758">Container Service (acs)</span></span>
- <span data-ttu-id="67fed-759">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="67fed-759">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="67fed-760">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="67fed-760">Networking</span></span>
- <span data-ttu-id="67fed-761">Storage</span><span class="sxs-lookup"><span data-stu-id="67fed-761">Storage</span></span>

<span data-ttu-id="67fed-762">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="67fed-762">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="67fed-763">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="67fed-763">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="67fed-764">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="67fed-764">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="67fed-765">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="67fed-765">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="67fed-766">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="67fed-766">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="67fed-767">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="67fed-767">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="67fed-768">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="67fed-768">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="67fed-769">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="67fed-769">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="67fed-770">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="67fed-770">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="67fed-771">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="67fed-771">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="67fed-772">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="67fed-772">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="67fed-773">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="67fed-773">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="67fed-774">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="67fed-774">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="67fed-775">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="67fed-775">Provide feedback from the command line with the `az feedback` command.</span></span>

