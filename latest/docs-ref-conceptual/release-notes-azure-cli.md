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
ms.openlocfilehash: 429b099dabd27d9356e88791f955ec52acd2a5f9
ms.sourcegitcommit: 9b36c15dc0e10024e23b8018604f5ef63c025de1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/24/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="c6cf4-104">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="c6cf4-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c6cf4-105">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-105">October 24, 2017</span></span>

<span data-ttu-id="c6cf4-106">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c6cf4-106">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c6cf4-107">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-107">Core</span></span>

* <span data-ttu-id="c6cf4-108">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="c6cf4-108">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c6cf4-109">ACR</span><span class="sxs-lookup"><span data-stu-id="c6cf4-109">ACR</span></span>

* <span data-ttu-id="c6cf4-110">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-110">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c6cf4-111">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-111">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c6cf4-112">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-112">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-113">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-113">ACS</span></span>

* <span data-ttu-id="c6cf4-114">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-114">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c6cf4-115">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-115">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-116">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-116">Appservice</span></span>

* <span data-ttu-id="c6cf4-117">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="c6cf4-117">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c6cf4-118">Komponente</span><span class="sxs-lookup"><span data-stu-id="c6cf4-118">Component</span></span>

* <span data-ttu-id="c6cf4-119">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-119">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c6cf4-120">Überwachen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-120">Monitor</span></span>

* <span data-ttu-id="c6cf4-121">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-121">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-122">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-122">Resource</span></span>

* <span data-ttu-id="c6cf4-123">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-123">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c6cf4-124">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="c6cf4-124">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-125">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-125">VM</span></span>

* <span data-ttu-id="c6cf4-126">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-126">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c6cf4-127">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-127">October 9, 2017</span></span>

<span data-ttu-id="c6cf4-128">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c6cf4-128">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c6cf4-129">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-129">Core</span></span>

* <span data-ttu-id="c6cf4-130">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-130">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-131">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-131">Appservice</span></span>

* <span data-ttu-id="c6cf4-132">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-132">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c6cf4-133">Batch</span><span class="sxs-lookup"><span data-stu-id="c6cf4-133">Batch</span></span>

* <span data-ttu-id="c6cf4-134">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c6cf4-134">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c6cf4-135">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-135">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c6cf4-136">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-136">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c6cf4-137">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-137">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c6cf4-138">BatchAI</span><span class="sxs-lookup"><span data-stu-id="c6cf4-138">Batchai</span></span>

* <span data-ttu-id="c6cf4-139">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-139">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6cf4-140">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6cf4-140">Keyvault</span></span>

* <span data-ttu-id="c6cf4-141">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-141">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c6cf4-142">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-142">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c6cf4-143">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-143">Network</span></span>

* <span data-ttu-id="c6cf4-144">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-144">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c6cf4-145">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-145">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-146">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-146">Resource</span></span>

* <span data-ttu-id="c6cf4-147">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-147">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c6cf4-148">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-148">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c6cf4-149">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-149">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c6cf4-150">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-150">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c6cf4-151">Sql</span><span class="sxs-lookup"><span data-stu-id="c6cf4-151">Sql</span></span>

* <span data-ttu-id="c6cf4-152">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-152">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c6cf4-153">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-153">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c6cf4-154">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-154">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-155">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-155">Storage</span></span>

* <span data-ttu-id="c6cf4-156">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-156">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-157">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-157">Vm</span></span>

* <span data-ttu-id="c6cf4-158">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-158">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c6cf4-159">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-159">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c6cf4-160">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-160">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c6cf4-161">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-161">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c6cf4-162">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-162">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c6cf4-163">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-163">September 22, 2017</span></span>

<span data-ttu-id="c6cf4-164">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c6cf4-164">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-165">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-165">Resource</span></span>

* <span data-ttu-id="c6cf4-166">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-166">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c6cf4-167">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-167">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c6cf4-168">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-168">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c6cf4-169">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-169">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-170">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-170">Network</span></span>

* <span data-ttu-id="c6cf4-171">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-171">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c6cf4-172">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-172">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c6cf4-173">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-173">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c6cf4-174">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-174">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c6cf4-175">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-175">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c6cf4-176">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-176">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c6cf4-177">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-177">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-178">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-178">Storage</span></span>

* <span data-ttu-id="c6cf4-179">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-179">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c6cf4-180">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="c6cf4-180">Eventgrid</span></span>

* <span data-ttu-id="c6cf4-181">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-181">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c6cf4-182">SQL</span><span class="sxs-lookup"><span data-stu-id="c6cf4-182">SQL</span></span>

* <span data-ttu-id="c6cf4-183">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-183">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c6cf4-184">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-184">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c6cf4-185">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-185">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6cf4-186">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6cf4-186">Keyvault</span></span>

* <span data-ttu-id="c6cf4-187">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-187">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-188">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-188">VM</span></span>

* <span data-ttu-id="c6cf4-189">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-189">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c6cf4-190">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-190">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c6cf4-191">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-191">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c6cf4-192">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-192">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c6cf4-193">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-193">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c6cf4-194">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-194">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-195">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-195">ACS</span></span>

* <span data-ttu-id="c6cf4-196">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-196">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-197">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-197">Appservice</span></span>

* <span data-ttu-id="c6cf4-198">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-198">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c6cf4-199">Backup </span><span class="sxs-lookup"><span data-stu-id="c6cf4-199">Backup</span></span>

* <span data-ttu-id="c6cf4-200">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="c6cf4-200">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c6cf4-201">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-201">September 11, 2017</span></span>

<span data-ttu-id="c6cf4-202">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c6cf4-202">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c6cf4-203">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-203">Core</span></span>

* <span data-ttu-id="c6cf4-204">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-204">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c6cf4-205">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="c6cf4-205">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-206">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-206">Acs</span></span>

* <span data-ttu-id="c6cf4-207">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-207">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c6cf4-208">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-208">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-209">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-209">Appservice</span></span>

* <span data-ttu-id="c6cf4-210">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="c6cf4-210">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c6cf4-211">CDN</span><span class="sxs-lookup"><span data-stu-id="c6cf4-211">CDN</span></span>

* <span data-ttu-id="c6cf4-212">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-212">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="c6cf4-213">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="c6cf4-213">Extension</span></span>

* <span data-ttu-id="c6cf4-214">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-214">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6cf4-215">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6cf4-215">Keyvault</span></span>

* <span data-ttu-id="c6cf4-216">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="c6cf4-216">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-217">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-217">Network</span></span>

* <span data-ttu-id="c6cf4-218">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-218">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c6cf4-219">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-219">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c6cf4-220">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-220">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c6cf4-221">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c6cf4-222">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-222">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-223">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-223">Resource</span></span>

* <span data-ttu-id="c6cf4-224">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-224">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c6cf4-225">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-225">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c6cf4-226">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-226">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c6cf4-227">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="c6cf4-227">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c6cf4-228">SQL</span><span class="sxs-lookup"><span data-stu-id="c6cf4-228">SQL</span></span>

* <span data-ttu-id="c6cf4-229">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-229">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-230">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-230">VM</span></span>

* <span data-ttu-id="c6cf4-231">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="c6cf4-231">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c6cf4-232">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-232">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c6cf4-233">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-233">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c6cf4-234">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-234">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c6cf4-235">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-235">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c6cf4-236">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-236">August 31, 2017</span></span>

<span data-ttu-id="c6cf4-237">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c6cf4-237">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6cf4-238">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6cf4-238">Keyvault</span></span>

* <span data-ttu-id="c6cf4-239">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-239">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c6cf4-240">Sf</span><span class="sxs-lookup"><span data-stu-id="c6cf4-240">Sf</span></span>

* <span data-ttu-id="c6cf4-241">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-241">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-242">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-242">Storage</span></span>

* <span data-ttu-id="c6cf4-243">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-243">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c6cf4-244">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="c6cf4-244">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c6cf4-245">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-245">August 28, 2017</span></span>

<span data-ttu-id="c6cf4-246">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c6cf4-246">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c6cf4-247">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-247">CLI</span></span>

* <span data-ttu-id="c6cf4-248">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-248">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-249">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-249">ACS</span></span>

* <span data-ttu-id="c6cf4-250">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-250">Corrected preview regions.</span></span>
* <span data-ttu-id="c6cf4-251">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-251">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="c6cf4-252">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-252">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-253">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-253">Appservice</span></span>

* <span data-ttu-id="c6cf4-254">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-254">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c6cf4-255">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-255">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c6cf4-256">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-256">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c6cf4-257">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-257">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c6cf4-258">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-258">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c6cf4-259">IoT</span><span class="sxs-lookup"><span data-stu-id="c6cf4-259">IoT</span></span>

* <span data-ttu-id="c6cf4-260">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="c6cf4-260">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-261">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-261">Network</span></span>

* <span data-ttu-id="c6cf4-262">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-262">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c6cf4-263">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-263">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c6cf4-264">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-264">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c6cf4-265">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-265">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c6cf4-266">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-266">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c6cf4-267">Profil</span><span class="sxs-lookup"><span data-stu-id="c6cf4-267">Profile</span></span>

* <span data-ttu-id="c6cf4-268">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-268">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c6cf4-269">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c6cf4-269">Service Fabric</span></span>

* <span data-ttu-id="c6cf4-270">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="c6cf4-270">Preview release</span></span>
* <span data-ttu-id="c6cf4-271">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-271">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c6cf4-272">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-272">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c6cf4-273">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-273">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-274">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-274">Storage</span></span>

* <span data-ttu-id="c6cf4-275">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-275">Enabled setting blob tier</span></span>
* <span data-ttu-id="c6cf4-276">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-276">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c6cf4-277">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-277">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="c6cf4-278">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-278">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c6cf4-279">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-279">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c6cf4-280">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-280">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-281">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-281">VM</span></span>

* <span data-ttu-id="c6cf4-282">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-282">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c6cf4-283">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-283">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="c6cf4-284">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-284">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="c6cf4-285">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-285">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c6cf4-286">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-286">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c6cf4-287">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-287">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c6cf4-288">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-288">August 15, 2017</span></span>

<span data-ttu-id="c6cf4-289">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c6cf4-289">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-290">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-290">ACS</span></span>

* <span data-ttu-id="c6cf4-291">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-291">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-292">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-292">Appservice</span></span>

* <span data-ttu-id="c6cf4-293">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-293">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c6cf4-294">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c6cf4-294">Event Grid</span></span>

* <span data-ttu-id="c6cf4-295">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-295">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c6cf4-296">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-296">August 11, 2017</span></span>

<span data-ttu-id="c6cf4-297">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c6cf4-297">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-298">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-298">ACS</span></span>

* <span data-ttu-id="c6cf4-299">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-299">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c6cf4-300">Batch</span><span class="sxs-lookup"><span data-stu-id="c6cf4-300">Batch</span></span>

* <span data-ttu-id="c6cf4-301">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-301">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c6cf4-302">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-302">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c6cf4-303">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-303">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c6cf4-304">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-304">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c6cf4-305">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="c6cf4-305">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c6cf4-306">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-306">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c6cf4-307">Komponente</span><span class="sxs-lookup"><span data-stu-id="c6cf4-307">Component</span></span>

* <span data-ttu-id="c6cf4-308">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-308">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c6cf4-309">Container</span><span class="sxs-lookup"><span data-stu-id="c6cf4-309">Container</span></span>

* <span data-ttu-id="c6cf4-310">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="c6cf4-310">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c6cf4-311">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-311">Data Lake Store</span></span>

* <span data-ttu-id="c6cf4-312">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-312">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c6cf4-313">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c6cf4-313">Event Grid</span></span>

* <span data-ttu-id="c6cf4-314">Erste Version</span><span class="sxs-lookup"><span data-stu-id="c6cf4-314">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-315">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-315">Network</span></span>

* <span data-ttu-id="c6cf4-316">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-316">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c6cf4-317">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="c6cf4-317">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c6cf4-318">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-318">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c6cf4-319">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-319">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c6cf4-320">Profil</span><span class="sxs-lookup"><span data-stu-id="c6cf4-320">Profile</span></span>

* <span data-ttu-id="c6cf4-321">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="c6cf4-321">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-322">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-322">Storage</span></span>

* <span data-ttu-id="c6cf4-323">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-323">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-324">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-324">VM</span></span>

* <span data-ttu-id="c6cf4-325">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-325">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c6cf4-326">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-326">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c6cf4-327">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-327">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c6cf4-328">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="c6cf4-328">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c6cf4-329">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-329">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c6cf4-330">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-330">July 28, 2017</span></span>

<span data-ttu-id="c6cf4-331">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c6cf4-331">Version 2.0.12</span></span>

* <span data-ttu-id="c6cf4-332">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-332">Added container commands</span></span>
* <span data-ttu-id="c6cf4-333">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-333">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c6cf4-334">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-334">Core</span></span>

* <span data-ttu-id="c6cf4-335">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-335">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c6cf4-336">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-336">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c6cf4-337">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="c6cf4-337">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c6cf4-338">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-338">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c6cf4-339">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-339">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c6cf4-340">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-340">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c6cf4-341">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-341">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c6cf4-342">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-342">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c6cf4-343">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-343">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c6cf4-344">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="c6cf4-344">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c6cf4-345">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="c6cf4-345">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c6cf4-346">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-346">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c6cf4-347">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-347">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c6cf4-348">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-348">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c6cf4-349">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c6cf4-349">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c6cf4-350">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-350">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c6cf4-351">ACR</span><span class="sxs-lookup"><span data-stu-id="c6cf4-351">ACR</span></span>

* <span data-ttu-id="c6cf4-352">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-352">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c6cf4-353">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-353">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c6cf4-354">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-354">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c6cf4-355">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-355">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c6cf4-356">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-356">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c6cf4-357">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-357">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-358">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-358">ACS</span></span>

* <span data-ttu-id="c6cf4-359">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c6cf4-359">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-360">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-360">Appservice</span></span>

* <span data-ttu-id="c6cf4-361">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="c6cf4-361">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c6cf4-362">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="c6cf4-362">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c6cf4-363">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-363">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c6cf4-364">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-364">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c6cf4-365">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-365">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c6cf4-366">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-366">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c6cf4-367">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-367">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c6cf4-368">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-368">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c6cf4-369">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-369">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c6cf4-370">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-370">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c6cf4-371">Batch</span><span class="sxs-lookup"><span data-stu-id="c6cf4-371">Batch</span></span>

* <span data-ttu-id="c6cf4-372">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-372">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c6cf4-373">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-373">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c6cf4-374">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-374">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c6cf4-375">CDN</span><span class="sxs-lookup"><span data-stu-id="c6cf4-375">CDN</span></span>

* <span data-ttu-id="c6cf4-376">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="c6cf4-376">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="c6cf4-377">Cloud</span><span class="sxs-lookup"><span data-stu-id="c6cf4-377">Cloud</span></span>

* <span data-ttu-id="c6cf4-378">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-378">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c6cf4-379">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6cf4-379">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c6cf4-380">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-380">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c6cf4-381">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="c6cf4-381">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c6cf4-382">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-382">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c6cf4-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c6cf4-383">CosmosDB</span></span>

* <span data-ttu-id="c6cf4-384">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-384">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c6cf4-385">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-385">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c6cf4-386">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c6cf4-386">Data Lake Analytics</span></span>

* <span data-ttu-id="c6cf4-387">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-387">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c6cf4-388">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-388">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c6cf4-389">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-389">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c6cf4-390">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-390">Data Lake Store</span></span>

* <span data-ttu-id="c6cf4-391">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-391">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c6cf4-392">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="c6cf4-392">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c6cf4-393">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-393">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c6cf4-394">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-394">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c6cf4-395">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="c6cf4-395">Interactive</span></span>

* <span data-ttu-id="c6cf4-396">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-396">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c6cf4-397">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-397">Increased test coverage</span></span>
* <span data-ttu-id="c6cf4-398">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="c6cf4-398">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c6cf4-399">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-399">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c6cf4-400">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-400">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c6cf4-401">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-401">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c6cf4-402">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-402">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c6cf4-403">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-403">Added `--progress` flag</span></span>
* <span data-ttu-id="c6cf4-404">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-404">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c6cf4-405">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-405">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c6cf4-406">IoT</span><span class="sxs-lookup"><span data-stu-id="c6cf4-406">IoT</span></span>

* <span data-ttu-id="c6cf4-407">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="c6cf4-407">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c6cf4-408">(3934)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-408">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c6cf4-409">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="c6cf4-409">Key vault</span></span>

* <span data-ttu-id="c6cf4-410">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-410">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c6cf4-411">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-411">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c6cf4-412">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-412">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c6cf4-413">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-413">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c6cf4-414">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-414">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c6cf4-415">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-415">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c6cf4-416">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-416">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c6cf4-417">(3307)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-417">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c6cf4-418">Labor</span><span class="sxs-lookup"><span data-stu-id="c6cf4-418">Lab</span></span>

* <span data-ttu-id="c6cf4-419">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-419">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c6cf4-420">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-420">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c6cf4-421">Überwachen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-421">Monitor</span></span>

* <span data-ttu-id="c6cf4-422">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-422">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c6cf4-423">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-423">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c6cf4-424">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-424">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c6cf4-425">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-425">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c6cf4-426">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-426">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c6cf4-427">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-427">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c6cf4-428">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-428">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c6cf4-429">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-429">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c6cf4-430">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6cf4-430">`location` no longer required</span></span>
  * <span data-ttu-id="c6cf4-431">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="c6cf4-431">Add name and ID support for target</span></span>
  * <span data-ttu-id="c6cf4-432">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-432">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c6cf4-433">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-433">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c6cf4-434">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-434">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c6cf4-435">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="c6cf4-435">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c6cf4-436">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-436">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c6cf4-437">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-437">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-438">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-438">Network</span></span>

* <span data-ttu-id="c6cf4-439">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-439">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c6cf4-440">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-440">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c6cf4-441">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-441">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c6cf4-442">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-442">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c6cf4-443">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="c6cf4-443">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c6cf4-444">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-444">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c6cf4-445">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-445">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c6cf4-446">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-446">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c6cf4-447">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-447">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c6cf4-448">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-448">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c6cf4-449">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-449">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c6cf4-450">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-450">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c6cf4-451">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-451">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c6cf4-452">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-452">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c6cf4-453">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-453">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c6cf4-454">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-454">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c6cf4-455">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-455">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c6cf4-456">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="c6cf4-456">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c6cf4-457">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-457">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c6cf4-458">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-458">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c6cf4-459">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-459">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c6cf4-460">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-460">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c6cf4-461">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-461">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c6cf4-462">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-462">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c6cf4-463">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-463">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c6cf4-464">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-464">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c6cf4-465">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-465">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c6cf4-466">Profil</span><span class="sxs-lookup"><span data-stu-id="c6cf4-466">Profile</span></span>

* <span data-ttu-id="c6cf4-467">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="c6cf4-467">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c6cf4-468">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="c6cf4-468">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c6cf4-469">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-469">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c6cf4-470">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-470">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c6cf4-471">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="c6cf4-471">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c6cf4-472">RDBMS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-472">RDBMS</span></span>

* <span data-ttu-id="c6cf4-473">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-473">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c6cf4-474">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-474">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c6cf4-475">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-475">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c6cf4-476">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-476">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-477">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-477">Resource</span></span>

* <span data-ttu-id="c6cf4-478">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-478">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c6cf4-479">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="c6cf4-479">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c6cf4-480">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-480">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c6cf4-481">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-481">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c6cf4-482">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-482">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c6cf4-483">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-483">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c6cf4-484">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-484">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c6cf4-485">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-485">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c6cf4-486">Rolle</span><span class="sxs-lookup"><span data-stu-id="c6cf4-486">Role</span></span>

* <span data-ttu-id="c6cf4-487">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-487">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c6cf4-488">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-488">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c6cf4-489">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="c6cf4-489">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c6cf4-490">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-490">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c6cf4-491">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-491">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c6cf4-492">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c6cf4-492">Service Fabric</span></span>
* <span data-ttu-id="c6cf4-493">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-493">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c6cf4-494">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-494">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c6cf4-495">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-495">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c6cf4-496">SQL</span><span class="sxs-lookup"><span data-stu-id="c6cf4-496">SQL</span></span>

* <span data-ttu-id="c6cf4-497">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-497">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c6cf4-498">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-498">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c6cf4-499">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-499">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-500">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-500">Storage</span></span>

* <span data-ttu-id="c6cf4-501">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-501">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c6cf4-502">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-502">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c6cf4-503">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-503">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c6cf4-504">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-504">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="c6cf4-505">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-505">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="c6cf4-506">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-506">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-507">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-507">VM</span></span>

* <span data-ttu-id="c6cf4-508">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c6cf4-508">Support configuring nsg</span></span>
* <span data-ttu-id="c6cf4-509">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="c6cf4-509">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c6cf4-510">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-510">Support managed service identities</span></span>
* <span data-ttu-id="c6cf4-511">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-511">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="c6cf4-512">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-512">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c6cf4-513">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-513">May 10, 2017</span></span>

<span data-ttu-id="c6cf4-514">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c6cf4-514">Version 2.0.6</span></span>

* <span data-ttu-id="c6cf4-515">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-515">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c6cf4-516">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-516">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c6cf4-517">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="c6cf4-517">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="c6cf4-518">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-518">Include Cognitive Services module.</span></span>
* <span data-ttu-id="c6cf4-519">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-519">Include Service Fabric module.</span></span>
* <span data-ttu-id="c6cf4-520">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-520">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="c6cf4-521">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="c6cf4-521">Add support for CDN commands.</span></span>
* <span data-ttu-id="c6cf4-522">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-522">Remove Container module.</span></span>
* <span data-ttu-id="c6cf4-523">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-523">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c6cf4-524">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-524">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c6cf4-525">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-525">Core</span></span>

* <span data-ttu-id="c6cf4-526">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-526">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="c6cf4-527">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-527">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c6cf4-528">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-528">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c6cf4-529">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-529">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c6cf4-530">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-530">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c6cf4-531">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-531">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c6cf4-532">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-532">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c6cf4-533">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-533">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c6cf4-534">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-534">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c6cf4-535">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-535">core: Improved performance</span></span>
* <span data-ttu-id="c6cf4-536">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-536">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c6cf4-537">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="c6cf4-537">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c6cf4-538">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-538">ACS</span></span>

* <span data-ttu-id="c6cf4-539">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6cf4-539">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c6cf4-540">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-540">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c6cf4-541">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-541">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c6cf4-542">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-542">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c6cf4-543">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-543">AppService</span></span>

* <span data-ttu-id="c6cf4-544">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-544">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c6cf4-545">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-545">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c6cf4-546">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-546">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c6cf4-547">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="c6cf4-547">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c6cf4-548">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-548">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c6cf4-549">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-549">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c6cf4-550">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="c6cf4-550">support slot swap with preview</span></span>
* <span data-ttu-id="c6cf4-551">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-551">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c6cf4-552">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-552">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c6cf4-553">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c6cf4-553">CosmosDB</span></span>

* <span data-ttu-id="c6cf4-554">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-554">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="c6cf4-555">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-555">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c6cf4-556">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-556">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c6cf4-557">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="c6cf4-557">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c6cf4-558">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c6cf4-558">Data Lake Analytics</span></span>

* <span data-ttu-id="c6cf4-559">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="c6cf4-559">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="c6cf4-560">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-560">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c6cf4-561">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-561">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c6cf4-562">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="c6cf4-562">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c6cf4-563">Table</span><span class="sxs-lookup"><span data-stu-id="c6cf4-563">Table</span></span>
  * <span data-ttu-id="c6cf4-564">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="c6cf4-564">Table valued function</span></span>
  * <span data-ttu-id="c6cf4-565">Sicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-565">View</span></span>
  * <span data-ttu-id="c6cf4-566">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-566">Table Statistics.</span></span> <span data-ttu-id="c6cf4-567">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-567">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c6cf4-568">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c6cf4-568">Data Lake Store</span></span>

* <span data-ttu-id="c6cf4-569">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="c6cf4-569">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="c6cf4-570">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-570">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c6cf4-571">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="c6cf4-571">missed help for access show.</span></span> <span data-ttu-id="c6cf4-572">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c6cf4-572">adding it.</span></span> <span data-ttu-id="c6cf4-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c6cf4-574">Suchen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-574">Find</span></span>

* <span data-ttu-id="c6cf4-575">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="c6cf4-575">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6cf4-576">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6cf4-576">KeyVault</span></span>

* <span data-ttu-id="c6cf4-577">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-577">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c6cf4-578">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-578">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="c6cf4-579">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="c6cf4-579">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c6cf4-580">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="c6cf4-580">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="c6cf4-581">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-581">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c6cf4-582">Labor</span><span class="sxs-lookup"><span data-stu-id="c6cf4-582">Lab</span></span>

* <span data-ttu-id="c6cf4-583">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="c6cf4-583">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="c6cf4-584">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="c6cf4-584">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="c6cf4-585">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="c6cf4-585">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="c6cf4-586">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="c6cf4-586">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="c6cf4-587">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="c6cf4-587">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="c6cf4-588">Überwachen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-588">Monitor</span></span>

* <span data-ttu-id="c6cf4-589">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-589">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c6cf4-590">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-590">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c6cf4-591">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-591">Network</span></span>

* <span data-ttu-id="c6cf4-592">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-592">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="c6cf4-593">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-593">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="c6cf4-594">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="c6cf4-594">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="c6cf4-595">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-595">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="c6cf4-596">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="c6cf4-596">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="c6cf4-597">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="c6cf4-597">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="c6cf4-598">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-598">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="c6cf4-599">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-599">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="c6cf4-600">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-600">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="c6cf4-601">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="c6cf4-601">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c6cf4-602">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-602">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="c6cf4-603">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-603">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="c6cf4-604">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="c6cf4-604">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="c6cf4-605">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="c6cf4-605">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="c6cf4-606">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="c6cf4-606">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="c6cf4-607">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-607">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="c6cf4-608">Profil</span><span class="sxs-lookup"><span data-stu-id="c6cf4-608">Profile</span></span>

* <span data-ttu-id="c6cf4-609">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-609">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c6cf4-610">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-610">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c6cf4-611">Redis</span><span class="sxs-lookup"><span data-stu-id="c6cf4-611">Redis</span></span>

* <span data-ttu-id="c6cf4-612">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="c6cf4-612">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c6cf4-613">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-613">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="c6cf4-614">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6cf4-614">Resource</span></span>

* <span data-ttu-id="c6cf4-615">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-615">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c6cf4-616">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-616">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c6cf4-617">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-617">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c6cf4-618">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="c6cf4-618">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c6cf4-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c6cf4-620">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-620">Add docs for az lock update.</span></span> <span data-ttu-id="c6cf4-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c6cf4-622">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-622">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c6cf4-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c6cf4-624">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="c6cf4-624">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c6cf4-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c6cf4-626">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-626">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c6cf4-627">Rolle</span><span class="sxs-lookup"><span data-stu-id="c6cf4-627">Role</span></span>

* <span data-ttu-id="c6cf4-628">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-628">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c6cf4-629">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-629">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c6cf4-630">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-630">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c6cf4-631">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="c6cf4-631">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c6cf4-632">SQL</span><span class="sxs-lookup"><span data-stu-id="c6cf4-632">SQL</span></span>

* <span data-ttu-id="c6cf4-633">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-633">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="c6cf4-634">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-634">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c6cf4-635">Speicher</span><span class="sxs-lookup"><span data-stu-id="c6cf4-635">Storage</span></span>

* <span data-ttu-id="c6cf4-636">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-636">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="c6cf4-637">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="c6cf4-637">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c6cf4-638">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="c6cf4-638">Add support for large block blob upload</span></span>
* <span data-ttu-id="c6cf4-639">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="c6cf4-639">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-640">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-640">VM</span></span>

* <span data-ttu-id="c6cf4-641">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="c6cf4-641">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c6cf4-642">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-642">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c6cf4-643">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c6cf4-643">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c6cf4-644">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-644">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c6cf4-645">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-645">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c6cf4-646">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="c6cf4-646">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c6cf4-647">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-647">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c6cf4-648">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-648">April 3, 2017</span></span>

<span data-ttu-id="c6cf4-649">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c6cf4-649">Version 2.0.2</span></span>

<span data-ttu-id="c6cf4-650">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-650">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="c6cf4-651">Core</span><span class="sxs-lookup"><span data-stu-id="c6cf4-651">Core</span></span>

* <span data-ttu-id="c6cf4-652">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="c6cf4-652">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="c6cf4-653">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-653">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c6cf4-654">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-654">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c6cf4-655">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-655">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c6cf4-656">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-656">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c6cf4-657">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="c6cf4-657">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c6cf4-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c6cf4-659">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-659">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c6cf4-660">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="c6cf4-660">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="c6cf4-661">ACS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-661">ACS</span></span>

* <span data-ttu-id="c6cf4-662">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-662">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c6cf4-663">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="c6cf4-663">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c6cf4-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c6cf4-665">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="c6cf4-665">Add support for windows clusters.</span></span> <span data-ttu-id="c6cf4-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c6cf4-667">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="c6cf4-667">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c6cf4-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="c6cf4-669">AppService</span><span class="sxs-lookup"><span data-stu-id="c6cf4-669">AppService</span></span>

* <span data-ttu-id="c6cf4-670">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-670">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c6cf4-671">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-671">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c6cf4-672">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-672">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c6cf4-673">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-673">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="c6cf4-674">DataLake</span><span class="sxs-lookup"><span data-stu-id="c6cf4-674">DataLake</span></span>

* <span data-ttu-id="c6cf4-675">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-675">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="c6cf4-676">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="c6cf4-676">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="c6cf4-677">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c6cf4-677">DocuemntDB</span></span>

* <span data-ttu-id="c6cf4-678">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-678">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c6cf4-679">VM</span><span class="sxs-lookup"><span data-stu-id="c6cf4-679">VM</span></span>

* <span data-ttu-id="c6cf4-680">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-680">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c6cf4-681">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-681">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c6cf4-682">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-682">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c6cf4-683">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-683">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c6cf4-684">VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-684">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c6cf4-685">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-685">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="c6cf4-686">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c6cf4-686">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c6cf4-687">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="c6cf4-687">February 27, 2017</span></span>

<span data-ttu-id="c6cf4-688">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c6cf4-688">Version 2.0.0</span></span>

<span data-ttu-id="c6cf4-689">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-689">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="c6cf4-690">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-690">General availability applies to these command modules:</span></span>
- <span data-ttu-id="c6cf4-691">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-691">Container Service (acs)</span></span>
- <span data-ttu-id="c6cf4-692">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-692">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c6cf4-693">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c6cf4-693">Networking</span></span>
- <span data-ttu-id="c6cf4-694">Storage</span><span class="sxs-lookup"><span data-stu-id="c6cf4-694">Storage</span></span>

<span data-ttu-id="c6cf4-695">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-695">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="c6cf4-696">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-696">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="c6cf4-697">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-697">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="c6cf4-698">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-698">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="c6cf4-699">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-699">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="c6cf4-700">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-700">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="c6cf4-701">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-701">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="c6cf4-702">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-702">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="c6cf4-703">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-703">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="c6cf4-704">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c6cf4-704">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="c6cf4-705">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="c6cf4-705">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c6cf4-706">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-706">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c6cf4-707">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="c6cf4-707">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="c6cf4-708">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="c6cf4-708">Provide feedback from the command line with the `az feedback` command.</span></span>

