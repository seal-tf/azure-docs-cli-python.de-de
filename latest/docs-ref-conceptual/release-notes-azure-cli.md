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
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="d4b60-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="d4b60-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="d4b60-105">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-105">October 9, 2017</span></span>

<span data-ttu-id="d4b60-106">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d4b60-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d4b60-107">Core</span><span class="sxs-lookup"><span data-stu-id="d4b60-107">Core</span></span>

* <span data-ttu-id="d4b60-108">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-109">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-109">Appservice</span></span>

* <span data-ttu-id="d4b60-110">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d4b60-111">Batch</span><span class="sxs-lookup"><span data-stu-id="d4b60-111">Batch</span></span>

* <span data-ttu-id="d4b60-112">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d4b60-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d4b60-113">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d4b60-114">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d4b60-115">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d4b60-116">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d4b60-116">Batchai</span></span>

* <span data-ttu-id="d4b60-117">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d4b60-118">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d4b60-118">Keyvault</span></span>

* <span data-ttu-id="d4b60-119">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="d4b60-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d4b60-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d4b60-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d4b60-121">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-121">Network</span></span>

* <span data-ttu-id="d4b60-122">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="d4b60-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d4b60-123">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d4b60-124">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4b60-124">Resource</span></span>

* <span data-ttu-id="d4b60-125">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d4b60-126">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d4b60-127">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d4b60-128">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d4b60-129">Sql</span><span class="sxs-lookup"><span data-stu-id="d4b60-129">Sql</span></span>

* <span data-ttu-id="d4b60-130">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d4b60-131">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d4b60-132">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-133">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-133">Storage</span></span>

* <span data-ttu-id="d4b60-134">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-135">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-135">Vm</span></span>

* <span data-ttu-id="d4b60-136">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="d4b60-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d4b60-137">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d4b60-138">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d4b60-139">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d4b60-140">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d4b60-141">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-141">September 22, 2017</span></span>

<span data-ttu-id="d4b60-142">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="d4b60-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d4b60-143">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4b60-143">Resource</span></span>

* <span data-ttu-id="d4b60-144">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d4b60-145">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d4b60-146">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d4b60-147">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="d4b60-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-148">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-148">Network</span></span>

* <span data-ttu-id="d4b60-149">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d4b60-150">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d4b60-151">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d4b60-152">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d4b60-153">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d4b60-154">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d4b60-155">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-156">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-156">Storage</span></span>

* <span data-ttu-id="d4b60-157">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d4b60-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d4b60-158">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="d4b60-158">Eventgrid</span></span>

* <span data-ttu-id="d4b60-159">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d4b60-160">SQL</span><span class="sxs-lookup"><span data-stu-id="d4b60-160">SQL</span></span>

* <span data-ttu-id="d4b60-161">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="d4b60-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d4b60-162">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4b60-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d4b60-163">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d4b60-164">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d4b60-164">Keyvault</span></span>

* <span data-ttu-id="d4b60-165">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-166">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-166">VM</span></span>

* <span data-ttu-id="d4b60-167">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d4b60-168">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d4b60-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d4b60-169">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d4b60-170">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d4b60-171">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d4b60-172">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-173">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-173">ACS</span></span>

* <span data-ttu-id="d4b60-174">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-175">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-175">Appservice</span></span>

* <span data-ttu-id="d4b60-176">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d4b60-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d4b60-177">Backup </span><span class="sxs-lookup"><span data-stu-id="d4b60-177">Backup</span></span>

* <span data-ttu-id="d4b60-178">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="d4b60-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d4b60-179">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-179">September 11, 2017</span></span>

<span data-ttu-id="d4b60-180">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d4b60-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d4b60-181">Core</span><span class="sxs-lookup"><span data-stu-id="d4b60-181">Core</span></span>

* <span data-ttu-id="d4b60-182">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="d4b60-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d4b60-183">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="d4b60-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-184">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-184">Acs</span></span>

* <span data-ttu-id="d4b60-185">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d4b60-186">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-187">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-187">Appservice</span></span>

* <span data-ttu-id="d4b60-188">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="d4b60-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d4b60-189">CDN</span><span class="sxs-lookup"><span data-stu-id="d4b60-189">CDN</span></span>

* <span data-ttu-id="d4b60-190">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d4b60-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="d4b60-191">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="d4b60-191">Extension</span></span>

* <span data-ttu-id="d4b60-192">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="d4b60-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="d4b60-193">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d4b60-193">Keyvault</span></span>

* <span data-ttu-id="d4b60-194">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="d4b60-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-195">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-195">Network</span></span>

* <span data-ttu-id="d4b60-196">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d4b60-197">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d4b60-198">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d4b60-199">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d4b60-200">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d4b60-201">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4b60-201">Resource</span></span>

* <span data-ttu-id="d4b60-202">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="d4b60-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d4b60-203">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="d4b60-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d4b60-204">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="d4b60-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d4b60-205">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="d4b60-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d4b60-206">SQL</span><span class="sxs-lookup"><span data-stu-id="d4b60-206">SQL</span></span>

* <span data-ttu-id="d4b60-207">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-208">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-208">VM</span></span>

* <span data-ttu-id="d4b60-209">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="d4b60-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d4b60-210">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="d4b60-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d4b60-211">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d4b60-212">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="d4b60-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d4b60-213">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="d4b60-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d4b60-214">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-214">August 31, 2017</span></span>

<span data-ttu-id="d4b60-215">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d4b60-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d4b60-216">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d4b60-216">Keyvault</span></span>

* <span data-ttu-id="d4b60-217">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="d4b60-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d4b60-218">Sf</span><span class="sxs-lookup"><span data-stu-id="d4b60-218">Sf</span></span>

* <span data-ttu-id="d4b60-219">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-220">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-220">Storage</span></span>

* <span data-ttu-id="d4b60-221">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="d4b60-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d4b60-222">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="d4b60-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d4b60-223">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-223">August 28, 2017</span></span>

<span data-ttu-id="d4b60-224">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d4b60-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d4b60-225">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="d4b60-225">CLI</span></span>

* <span data-ttu-id="d4b60-226">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-227">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-227">ACS</span></span>

* <span data-ttu-id="d4b60-228">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="d4b60-228">Corrected preview regions.</span></span>
* <span data-ttu-id="d4b60-229">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="d4b60-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="d4b60-230">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="d4b60-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-231">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-231">Appservice</span></span>

* <span data-ttu-id="d4b60-232">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d4b60-233">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d4b60-234">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d4b60-235">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="d4b60-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d4b60-236">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d4b60-237">IoT</span><span class="sxs-lookup"><span data-stu-id="d4b60-237">IoT</span></span>

* <span data-ttu-id="d4b60-238">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="d4b60-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-239">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-239">Network</span></span>

* <span data-ttu-id="d4b60-240">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d4b60-241">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d4b60-242">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d4b60-243">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d4b60-244">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d4b60-245">Profil</span><span class="sxs-lookup"><span data-stu-id="d4b60-245">Profile</span></span>

* <span data-ttu-id="d4b60-246">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d4b60-247">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d4b60-247">Service Fabric</span></span>

* <span data-ttu-id="d4b60-248">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="d4b60-248">Preview release</span></span>
* <span data-ttu-id="d4b60-249">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d4b60-250">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d4b60-251">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-252">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-252">Storage</span></span>

* <span data-ttu-id="d4b60-253">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="d4b60-254">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d4b60-255">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="d4b60-256">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d4b60-257">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d4b60-258">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="d4b60-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-259">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-259">VM</span></span>

* <span data-ttu-id="d4b60-260">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="d4b60-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d4b60-261">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d4b60-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="d4b60-262">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="d4b60-263">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="d4b60-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d4b60-264">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d4b60-265">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d4b60-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d4b60-266">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-266">August 15, 2017</span></span>

<span data-ttu-id="d4b60-267">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d4b60-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-268">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-268">ACS</span></span>

* <span data-ttu-id="d4b60-269">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-270">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-270">Appservice</span></span>

* <span data-ttu-id="d4b60-271">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d4b60-272">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d4b60-272">Event Grid</span></span>

* <span data-ttu-id="d4b60-273">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d4b60-274">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-274">August 11, 2017</span></span>

<span data-ttu-id="d4b60-275">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d4b60-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-276">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-276">ACS</span></span>

* <span data-ttu-id="d4b60-277">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d4b60-278">Batch</span><span class="sxs-lookup"><span data-stu-id="d4b60-278">Batch</span></span>

* <span data-ttu-id="d4b60-279">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d4b60-280">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d4b60-281">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d4b60-282">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="d4b60-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d4b60-283">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="d4b60-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d4b60-284">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d4b60-285">Komponente</span><span class="sxs-lookup"><span data-stu-id="d4b60-285">Component</span></span>

* <span data-ttu-id="d4b60-286">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d4b60-287">Container</span><span class="sxs-lookup"><span data-stu-id="d4b60-287">Container</span></span>

* <span data-ttu-id="d4b60-288">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="d4b60-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d4b60-289">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-289">Data Lake Store</span></span>

* <span data-ttu-id="d4b60-290">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d4b60-291">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d4b60-291">Event Grid</span></span>

* <span data-ttu-id="d4b60-292">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d4b60-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-293">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-293">Network</span></span>

* <span data-ttu-id="d4b60-294">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="d4b60-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d4b60-295">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="d4b60-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d4b60-296">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="d4b60-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d4b60-297">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="d4b60-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d4b60-298">Profil</span><span class="sxs-lookup"><span data-stu-id="d4b60-298">Profile</span></span>

* <span data-ttu-id="d4b60-299">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="d4b60-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-300">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-300">Storage</span></span>

* <span data-ttu-id="d4b60-301">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-302">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-302">VM</span></span>

* <span data-ttu-id="d4b60-303">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d4b60-304">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d4b60-305">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d4b60-306">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="d4b60-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d4b60-307">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d4b60-308">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-308">July 28, 2017</span></span>

<span data-ttu-id="d4b60-309">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d4b60-309">Version 2.0.12</span></span>

* <span data-ttu-id="d4b60-310">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-310">Added container commands</span></span>
* <span data-ttu-id="d4b60-311">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d4b60-312">Core</span><span class="sxs-lookup"><span data-stu-id="d4b60-312">Core</span></span>

* <span data-ttu-id="d4b60-313">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="d4b60-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d4b60-314">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d4b60-315">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="d4b60-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d4b60-316">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="d4b60-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d4b60-317">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="d4b60-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d4b60-318">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="d4b60-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d4b60-319">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="d4b60-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d4b60-320">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="d4b60-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d4b60-321">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="d4b60-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d4b60-322">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="d4b60-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d4b60-323">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="d4b60-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d4b60-324">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="d4b60-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d4b60-325">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="d4b60-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d4b60-326">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="d4b60-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d4b60-327">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d4b60-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d4b60-328">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="d4b60-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d4b60-329">ACR</span><span class="sxs-lookup"><span data-stu-id="d4b60-329">ACR</span></span>

* <span data-ttu-id="d4b60-330">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d4b60-331">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d4b60-332">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d4b60-333">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d4b60-334">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d4b60-335">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-336">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-336">ACS</span></span>

* <span data-ttu-id="d4b60-337">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="d4b60-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-338">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-338">Appservice</span></span>

* <span data-ttu-id="d4b60-339">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="d4b60-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d4b60-340">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="d4b60-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d4b60-341">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="d4b60-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d4b60-342">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="d4b60-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d4b60-343">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="d4b60-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d4b60-344">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="d4b60-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d4b60-345">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="d4b60-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d4b60-346">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="d4b60-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d4b60-347">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d4b60-348">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="d4b60-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d4b60-349">Batch</span><span class="sxs-lookup"><span data-stu-id="d4b60-349">Batch</span></span>

* <span data-ttu-id="d4b60-350">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d4b60-351">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d4b60-352">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d4b60-353">CDN</span><span class="sxs-lookup"><span data-stu-id="d4b60-353">CDN</span></span>

* <span data-ttu-id="d4b60-354">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="d4b60-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="d4b60-355">Cloud</span><span class="sxs-lookup"><span data-stu-id="d4b60-355">Cloud</span></span>

* <span data-ttu-id="d4b60-356">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="d4b60-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d4b60-357">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4b60-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d4b60-358">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="d4b60-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d4b60-359">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="d4b60-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d4b60-360">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d4b60-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d4b60-361">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d4b60-361">CosmosDB</span></span>

* <span data-ttu-id="d4b60-362">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="d4b60-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d4b60-363">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d4b60-364">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d4b60-364">Data Lake Analytics</span></span>

* <span data-ttu-id="d4b60-365">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d4b60-366">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d4b60-367">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d4b60-368">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-368">Data Lake Store</span></span>

* <span data-ttu-id="d4b60-369">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d4b60-370">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="d4b60-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d4b60-371">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d4b60-372">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="d4b60-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d4b60-373">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="d4b60-373">Interactive</span></span>

* <span data-ttu-id="d4b60-374">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="d4b60-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d4b60-375">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="d4b60-375">Increased test coverage</span></span>
* <span data-ttu-id="d4b60-376">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="d4b60-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d4b60-377">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="d4b60-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d4b60-378">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="d4b60-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d4b60-379">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="d4b60-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d4b60-380">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="d4b60-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d4b60-381">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-381">Added `--progress` flag</span></span>
* <span data-ttu-id="d4b60-382">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d4b60-383">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="d4b60-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d4b60-384">IoT</span><span class="sxs-lookup"><span data-stu-id="d4b60-384">IoT</span></span>

* <span data-ttu-id="d4b60-385">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="d4b60-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d4b60-386">(3934)</span><span class="sxs-lookup"><span data-stu-id="d4b60-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d4b60-387">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="d4b60-387">Key vault</span></span>

* <span data-ttu-id="d4b60-388">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d4b60-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d4b60-389">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d4b60-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d4b60-390">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d4b60-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d4b60-391">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d4b60-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d4b60-392">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d4b60-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d4b60-393">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="d4b60-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d4b60-394">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d4b60-395">(3307)</span><span class="sxs-lookup"><span data-stu-id="d4b60-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d4b60-396">Labor</span><span class="sxs-lookup"><span data-stu-id="d4b60-396">Lab</span></span>

* <span data-ttu-id="d4b60-397">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d4b60-398">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d4b60-399">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d4b60-399">Monitor</span></span>

* <span data-ttu-id="d4b60-400">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="d4b60-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d4b60-401">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d4b60-402">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d4b60-403">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d4b60-404">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="d4b60-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d4b60-405">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="d4b60-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d4b60-406">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="d4b60-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d4b60-407">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="d4b60-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d4b60-408">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4b60-408">`location` no longer required</span></span>
  * <span data-ttu-id="d4b60-409">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="d4b60-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="d4b60-410">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="d4b60-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d4b60-411">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="d4b60-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d4b60-412">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d4b60-413">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="d4b60-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d4b60-414">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="d4b60-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d4b60-415">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-416">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-416">Network</span></span>

* <span data-ttu-id="d4b60-417">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d4b60-418">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d4b60-419">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="d4b60-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d4b60-420">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="d4b60-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d4b60-421">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="d4b60-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d4b60-422">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d4b60-423">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d4b60-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d4b60-424">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d4b60-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d4b60-425">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d4b60-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d4b60-426">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d4b60-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d4b60-427">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d4b60-428">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d4b60-429">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d4b60-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d4b60-430">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d4b60-431">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d4b60-432">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d4b60-433">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d4b60-434">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="d4b60-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d4b60-435">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d4b60-436">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d4b60-437">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="d4b60-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d4b60-438">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="d4b60-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d4b60-439">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="d4b60-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d4b60-440">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d4b60-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d4b60-441">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d4b60-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d4b60-442">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d4b60-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d4b60-443">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="d4b60-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d4b60-444">Profil</span><span class="sxs-lookup"><span data-stu-id="d4b60-444">Profile</span></span>

* <span data-ttu-id="d4b60-445">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="d4b60-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d4b60-446">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="d4b60-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d4b60-447">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="d4b60-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d4b60-448">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d4b60-449">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="d4b60-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d4b60-450">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d4b60-450">RDBMS</span></span>

* <span data-ttu-id="d4b60-451">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="d4b60-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d4b60-452">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="d4b60-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d4b60-453">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="d4b60-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d4b60-454">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="d4b60-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d4b60-455">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4b60-455">Resource</span></span>

* <span data-ttu-id="d4b60-456">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="d4b60-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d4b60-457">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="d4b60-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d4b60-458">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="d4b60-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d4b60-459">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="d4b60-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d4b60-460">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="d4b60-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d4b60-461">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="d4b60-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d4b60-462">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="d4b60-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d4b60-463">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d4b60-464">Rolle</span><span class="sxs-lookup"><span data-stu-id="d4b60-464">Role</span></span>

* <span data-ttu-id="d4b60-465">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d4b60-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d4b60-466">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="d4b60-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d4b60-467">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="d4b60-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d4b60-468">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="d4b60-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d4b60-469">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d4b60-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d4b60-470">Service Fabric</span></span>
* <span data-ttu-id="d4b60-471">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="d4b60-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d4b60-472">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="d4b60-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d4b60-473">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="d4b60-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d4b60-474">SQL</span><span class="sxs-lookup"><span data-stu-id="d4b60-474">SQL</span></span>

* <span data-ttu-id="d4b60-475">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d4b60-476">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="d4b60-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d4b60-477">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-478">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-478">Storage</span></span>

* <span data-ttu-id="d4b60-479">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="d4b60-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d4b60-480">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d4b60-481">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="d4b60-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d4b60-482">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="d4b60-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="d4b60-483">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="d4b60-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="d4b60-484">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="d4b60-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-485">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-485">VM</span></span>

* <span data-ttu-id="d4b60-486">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d4b60-486">Support configuring nsg</span></span>
* <span data-ttu-id="d4b60-487">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="d4b60-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d4b60-488">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="d4b60-488">Support managed service identities</span></span>
* <span data-ttu-id="d4b60-489">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="d4b60-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="d4b60-490">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="d4b60-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d4b60-491">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-491">May 10, 2017</span></span>

<span data-ttu-id="d4b60-492">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d4b60-492">Version 2.0.6</span></span>

* <span data-ttu-id="d4b60-493">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="d4b60-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d4b60-494">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="d4b60-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d4b60-495">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="d4b60-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="d4b60-496">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="d4b60-497">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="d4b60-498">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="d4b60-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="d4b60-499">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="d4b60-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="d4b60-500">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-500">Remove Container module.</span></span>
* <span data-ttu-id="d4b60-501">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="d4b60-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d4b60-502">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d4b60-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d4b60-503">Core</span><span class="sxs-lookup"><span data-stu-id="d4b60-503">Core</span></span>

* <span data-ttu-id="d4b60-504">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="d4b60-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="d4b60-505">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d4b60-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d4b60-506">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d4b60-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d4b60-507">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d4b60-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d4b60-508">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d4b60-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d4b60-509">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d4b60-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d4b60-510">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d4b60-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d4b60-511">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d4b60-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d4b60-512">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d4b60-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d4b60-513">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="d4b60-513">core: Improved performance</span></span>
* <span data-ttu-id="d4b60-514">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="d4b60-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d4b60-515">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="d4b60-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d4b60-516">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-516">ACS</span></span>

* <span data-ttu-id="d4b60-517">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4b60-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d4b60-518">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="d4b60-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d4b60-519">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d4b60-520">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d4b60-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d4b60-521">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-521">AppService</span></span>

* <span data-ttu-id="d4b60-522">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="d4b60-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d4b60-523">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="d4b60-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d4b60-524">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="d4b60-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d4b60-525">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="d4b60-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d4b60-526">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="d4b60-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d4b60-527">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d4b60-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d4b60-528">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="d4b60-528">support slot swap with preview</span></span>
* <span data-ttu-id="d4b60-529">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d4b60-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d4b60-530">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d4b60-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d4b60-531">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d4b60-531">CosmosDB</span></span>

* <span data-ttu-id="d4b60-532">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="d4b60-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="d4b60-533">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="d4b60-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d4b60-534">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="d4b60-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d4b60-535">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="d4b60-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d4b60-536">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d4b60-536">Data Lake Analytics</span></span>

* <span data-ttu-id="d4b60-537">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="d4b60-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="d4b60-538">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="d4b60-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d4b60-539">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d4b60-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d4b60-540">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="d4b60-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d4b60-541">Table</span><span class="sxs-lookup"><span data-stu-id="d4b60-541">Table</span></span>
  * <span data-ttu-id="d4b60-542">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="d4b60-542">Table valued function</span></span>
  * <span data-ttu-id="d4b60-543">Sicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-543">View</span></span>
  * <span data-ttu-id="d4b60-544">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="d4b60-544">Table Statistics.</span></span> <span data-ttu-id="d4b60-545">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="d4b60-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d4b60-546">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d4b60-546">Data Lake Store</span></span>

* <span data-ttu-id="d4b60-547">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="d4b60-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="d4b60-548">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d4b60-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d4b60-549">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="d4b60-549">missed help for access show.</span></span> <span data-ttu-id="d4b60-550">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d4b60-550">adding it.</span></span> <span data-ttu-id="d4b60-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d4b60-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d4b60-552">Suchen</span><span class="sxs-lookup"><span data-stu-id="d4b60-552">Find</span></span>

* <span data-ttu-id="d4b60-553">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="d4b60-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d4b60-554">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d4b60-554">KeyVault</span></span>

* <span data-ttu-id="d4b60-555">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="d4b60-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d4b60-556">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="d4b60-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="d4b60-557">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="d4b60-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d4b60-558">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="d4b60-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="d4b60-559">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d4b60-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d4b60-560">Labor</span><span class="sxs-lookup"><span data-stu-id="d4b60-560">Lab</span></span>

* <span data-ttu-id="d4b60-561">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="d4b60-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="d4b60-562">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="d4b60-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="d4b60-563">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="d4b60-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="d4b60-564">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="d4b60-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="d4b60-565">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="d4b60-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="d4b60-566">Überwachen</span><span class="sxs-lookup"><span data-stu-id="d4b60-566">Monitor</span></span>

* <span data-ttu-id="d4b60-567">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d4b60-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d4b60-568">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d4b60-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d4b60-569">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-569">Network</span></span>

* <span data-ttu-id="d4b60-570">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="d4b60-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="d4b60-571">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="d4b60-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="d4b60-572">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="d4b60-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="d4b60-573">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="d4b60-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="d4b60-574">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="d4b60-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="d4b60-575">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="d4b60-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="d4b60-576">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="d4b60-577">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="d4b60-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="d4b60-578">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="d4b60-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="d4b60-579">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="d4b60-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d4b60-580">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="d4b60-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="d4b60-581">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d4b60-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="d4b60-582">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="d4b60-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="d4b60-583">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="d4b60-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="d4b60-584">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="d4b60-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="d4b60-585">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="d4b60-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="d4b60-586">Profil</span><span class="sxs-lookup"><span data-stu-id="d4b60-586">Profile</span></span>

* <span data-ttu-id="d4b60-587">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d4b60-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d4b60-588">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d4b60-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d4b60-589">Redis</span><span class="sxs-lookup"><span data-stu-id="d4b60-589">Redis</span></span>

* <span data-ttu-id="d4b60-590">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="d4b60-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d4b60-591">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="d4b60-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="d4b60-592">Ressource</span><span class="sxs-lookup"><span data-stu-id="d4b60-592">Resource</span></span>

* <span data-ttu-id="d4b60-593">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d4b60-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d4b60-594">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d4b60-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d4b60-595">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d4b60-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d4b60-596">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="d4b60-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d4b60-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d4b60-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d4b60-598">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="d4b60-598">Add docs for az lock update.</span></span> <span data-ttu-id="d4b60-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d4b60-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d4b60-600">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="d4b60-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d4b60-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d4b60-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d4b60-602">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="d4b60-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d4b60-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d4b60-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d4b60-604">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d4b60-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d4b60-605">Rolle</span><span class="sxs-lookup"><span data-stu-id="d4b60-605">Role</span></span>

* <span data-ttu-id="d4b60-606">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d4b60-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d4b60-607">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d4b60-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d4b60-608">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d4b60-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d4b60-609">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="d4b60-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d4b60-610">SQL</span><span class="sxs-lookup"><span data-stu-id="d4b60-610">SQL</span></span>

* <span data-ttu-id="d4b60-611">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="d4b60-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="d4b60-612">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d4b60-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d4b60-613">Speicher</span><span class="sxs-lookup"><span data-stu-id="d4b60-613">Storage</span></span>

* <span data-ttu-id="d4b60-614">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d4b60-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="d4b60-615">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="d4b60-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d4b60-616">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="d4b60-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="d4b60-617">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="d4b60-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-618">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-618">VM</span></span>

* <span data-ttu-id="d4b60-619">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="d4b60-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d4b60-620">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="d4b60-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d4b60-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d4b60-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d4b60-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d4b60-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d4b60-623">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="d4b60-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d4b60-624">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="d4b60-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d4b60-625">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d4b60-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d4b60-626">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-626">April 3, 2017</span></span>

<span data-ttu-id="d4b60-627">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d4b60-627">Version 2.0.2</span></span>

<span data-ttu-id="d4b60-628">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="d4b60-629">Core</span><span class="sxs-lookup"><span data-stu-id="d4b60-629">Core</span></span>

* <span data-ttu-id="d4b60-630">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="d4b60-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="d4b60-631">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d4b60-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d4b60-632">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d4b60-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d4b60-633">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d4b60-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d4b60-634">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d4b60-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d4b60-635">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="d4b60-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d4b60-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d4b60-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d4b60-637">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d4b60-638">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="d4b60-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="d4b60-639">ACS</span><span class="sxs-lookup"><span data-stu-id="d4b60-639">ACS</span></span>

* <span data-ttu-id="d4b60-640">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d4b60-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d4b60-641">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="d4b60-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d4b60-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d4b60-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d4b60-643">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="d4b60-643">Add support for windows clusters.</span></span> <span data-ttu-id="d4b60-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d4b60-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d4b60-645">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="d4b60-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d4b60-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d4b60-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="d4b60-647">AppService</span><span class="sxs-lookup"><span data-stu-id="d4b60-647">AppService</span></span>

* <span data-ttu-id="d4b60-648">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d4b60-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d4b60-649">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d4b60-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d4b60-650">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d4b60-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d4b60-651">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d4b60-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="d4b60-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="d4b60-652">DataLake</span></span>

* <span data-ttu-id="d4b60-653">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="d4b60-654">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="d4b60-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="d4b60-655">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d4b60-655">DocuemntDB</span></span>

* <span data-ttu-id="d4b60-656">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d4b60-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d4b60-657">VM</span><span class="sxs-lookup"><span data-stu-id="d4b60-657">VM</span></span>

* <span data-ttu-id="d4b60-658">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d4b60-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d4b60-659">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d4b60-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d4b60-660">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d4b60-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d4b60-661">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d4b60-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d4b60-662">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d4b60-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d4b60-663">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="d4b60-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="d4b60-664">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d4b60-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d4b60-665">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="d4b60-665">February 27, 2017</span></span>

<span data-ttu-id="d4b60-666">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d4b60-666">Version 2.0.0</span></span>

<span data-ttu-id="d4b60-667">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="d4b60-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="d4b60-668">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="d4b60-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="d4b60-669">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="d4b60-669">Container Service (acs)</span></span>
- <span data-ttu-id="d4b60-670">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d4b60-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d4b60-671">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="d4b60-671">Networking</span></span>
- <span data-ttu-id="d4b60-672">Storage</span><span class="sxs-lookup"><span data-stu-id="d4b60-672">Storage</span></span>

<span data-ttu-id="d4b60-673">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4b60-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="d4b60-674">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="d4b60-675">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="d4b60-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="d4b60-676">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="d4b60-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="d4b60-677">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="d4b60-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="d4b60-678">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="d4b60-679">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="d4b60-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="d4b60-680">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="d4b60-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="d4b60-681">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="d4b60-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="d4b60-682">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="d4b60-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="d4b60-683">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="d4b60-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d4b60-684">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d4b60-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d4b60-685">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d4b60-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="d4b60-686">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d4b60-686">Provide feedback from the command line with the `az feedback` command.</span></span>

