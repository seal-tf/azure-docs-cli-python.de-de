---
title: Azure CLI 2.0-Versionshinweise
description: "Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01078b7a3665f563f0a6b1d809c9a41f18d136d6
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="1a4c1-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="1a4c1-103">Azure CLI 2.0 release notes</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="1a4c1-104">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="1a4c1-104">February 27, 2018</span></span>

<span data-ttu-id="1a4c1-105">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="1a4c1-105">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-106">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-106">Core</span></span>

* <span data-ttu-id="1a4c1-107">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-107">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="1a4c1-108">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-108">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="1a4c1-109">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-109">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-110">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-110">ACS</span></span>

* <span data-ttu-id="1a4c1-111">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-111">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="1a4c1-112">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="1a4c1-112">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="1a4c1-113">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-113">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="1a4c1-114">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-114">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-115">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-115">Appservice</span></span>

* <span data-ttu-id="1a4c1-116">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-116">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="1a4c1-117">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-117">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1a4c1-118">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1a4c1-118">Cognitive Services</span></span>

* <span data-ttu-id="1a4c1-119">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-119">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="1a4c1-120">Nutzung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-120">Consumption</span></span>

* <span data-ttu-id="1a4c1-121">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-121">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="1a4c1-122">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-122">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-123">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-123">Container</span></span>

* <span data-ttu-id="1a4c1-124">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="1a4c1-124">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-125">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-125">Network</span></span>

* <span data-ttu-id="1a4c1-126">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-126">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-127">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-127">Resource</span></span>

* <span data-ttu-id="1a4c1-128">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="1a4c1-128">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-129">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-129">Role</span></span>

* <span data-ttu-id="1a4c1-130">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-130">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-131">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-131">SQL</span></span>

* <span data-ttu-id="1a4c1-132">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-132">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-133">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-133">Storage</span></span>

* <span data-ttu-id="1a4c1-134">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-134">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-135">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-135">VM</span></span>

* <span data-ttu-id="1a4c1-136">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-136">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="1a4c1-137">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="1a4c1-137">February 13, 2018</span></span>

<span data-ttu-id="1a4c1-138">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="1a4c1-138">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-139">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-139">Core</span></span>

* <span data-ttu-id="1a4c1-140">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-140">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-141">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-141">ACS</span></span>

* <span data-ttu-id="1a4c1-142">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-142">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="1a4c1-143">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-143">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="1a4c1-144">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-144">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="1a4c1-145">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-145">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="1a4c1-146">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-146">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="1a4c1-147">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-147">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="1a4c1-148">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="1a4c1-148">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="1a4c1-149">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="1a4c1-149">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-150">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-150">Appservice</span></span>

* <span data-ttu-id="1a4c1-151">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-151">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="1a4c1-152">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-152">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="1a4c1-153">CDN</span><span class="sxs-lookup"><span data-stu-id="1a4c1-153">CDN</span></span>

* <span data-ttu-id="1a4c1-154">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-154">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-155">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-155">Container</span></span>

* <span data-ttu-id="1a4c1-156">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-156">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="1a4c1-157">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-157">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1a4c1-158">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1a4c1-158">CosmosDB</span></span>

* <span data-ttu-id="1a4c1-159">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-159">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="1a4c1-160">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="1a4c1-160">Extension</span></span>

* <span data-ttu-id="1a4c1-161">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-161">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="1a4c1-162">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-162">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="1a4c1-163">Feedback</span><span class="sxs-lookup"><span data-stu-id="1a4c1-163">Feedback</span></span>

* <span data-ttu-id="1a4c1-164">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-164">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="1a4c1-165">Interactive</span><span class="sxs-lookup"><span data-stu-id="1a4c1-165">Interactive</span></span>

* <span data-ttu-id="1a4c1-166">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-166">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="1a4c1-167">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-167">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="1a4c1-168">IoT</span><span class="sxs-lookup"><span data-stu-id="1a4c1-168">IoT</span></span>

* <span data-ttu-id="1a4c1-169">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-169">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="1a4c1-170">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-170">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="1a4c1-171">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-171">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="1a4c1-172">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-172">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-173">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-173">Monitor</span></span>

* <span data-ttu-id="1a4c1-174">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-174">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-175">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-175">Network</span></span>

* <span data-ttu-id="1a4c1-176">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-176">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="1a4c1-177">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-177">Profile</span></span>

* <span data-ttu-id="1a4c1-178">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-178">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-179">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-179">Resource</span></span>

* <span data-ttu-id="1a4c1-180">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-180">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-181">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-181">Role</span></span>

* <span data-ttu-id="1a4c1-182">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-182">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-183">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-183">SQL</span></span>

* <span data-ttu-id="1a4c1-184">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-184">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="1a4c1-185">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-185">Added `sql db rename`</span></span>
* <span data-ttu-id="1a4c1-186">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-186">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-187">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-187">Storage</span></span>

* <span data-ttu-id="1a4c1-188">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-188">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-189">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-189">VM</span></span>

* <span data-ttu-id="1a4c1-190">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-190">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="1a4c1-191">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-191">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="1a4c1-192">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-192">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="1a4c1-193">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="1a4c1-193">January 31, 2018</span></span>

<span data-ttu-id="1a4c1-194">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="1a4c1-194">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-195">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-195">Core</span></span>

* <span data-ttu-id="1a4c1-196">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-196">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="1a4c1-197">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-197">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="1a4c1-198">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-198">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="1a4c1-199">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-199">Use `--verbose` to see</span></span>
* <span data-ttu-id="1a4c1-200">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-200">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-201">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-201">ACS</span></span>

* <span data-ttu-id="1a4c1-202">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-202">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="1a4c1-203">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-203">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-204">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-204">Appservice</span></span>

* <span data-ttu-id="1a4c1-205">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-205">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="1a4c1-206">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-206">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="1a4c1-207">CDN</span><span class="sxs-lookup"><span data-stu-id="1a4c1-207">CDN</span></span>

* <span data-ttu-id="1a4c1-208">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-208">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1a4c1-209">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1a4c1-209">CosmosDB</span></span>

* <span data-ttu-id="1a4c1-210">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-210">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="1a4c1-211">Interactive</span><span class="sxs-lookup"><span data-stu-id="1a4c1-211">Interactive</span></span>

* <span data-ttu-id="1a4c1-212">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-212">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-213">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-213">Network</span></span>

* <span data-ttu-id="1a4c1-214">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-214">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="1a4c1-215">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="1a4c1-215">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="1a4c1-216">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-216">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="1a4c1-217">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-217">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="1a4c1-218">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-218">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="1a4c1-219">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-219">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="1a4c1-220">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-220">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="1a4c1-221">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-221">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="1a4c1-222">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-222">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="1a4c1-223">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-223">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-224">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-224">Profile</span></span>

* <span data-ttu-id="1a4c1-225">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-225">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-226">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-226">Resource</span></span>

* <span data-ttu-id="1a4c1-227">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-227">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-228">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-228">Storage</span></span>

* <span data-ttu-id="1a4c1-229">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-229">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="1a4c1-230">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-230">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="1a4c1-231">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-231">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="1a4c1-232">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-232">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="1a4c1-233">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-233">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-234">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-234">VM</span></span>

* <span data-ttu-id="1a4c1-235">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-235">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="1a4c1-236">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="1a4c1-236">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="1a4c1-237">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-237">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="1a4c1-238">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-238">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="1a4c1-239">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="1a4c1-239">January 17, 2018</span></span>

<span data-ttu-id="1a4c1-240">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="1a4c1-240">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="1a4c1-241">ACR</span><span class="sxs-lookup"><span data-stu-id="1a4c1-241">ACR</span></span>

* <span data-ttu-id="1a4c1-242">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-242">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="1a4c1-243">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-243">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-244">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-244">ACS</span></span>

* <span data-ttu-id="1a4c1-245">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-245">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="1a4c1-246">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-246">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-247">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-247">Appservice</span></span>

* <span data-ttu-id="1a4c1-248">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="1a4c1-248">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="1a4c1-249">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-249">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="1a4c1-250">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-250">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="1a4c1-251">Sicherung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-251">Backup</span></span>

* <span data-ttu-id="1a4c1-252">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-252">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="1a4c1-253">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-253">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="1a4c1-254">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-254">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="1a4c1-255">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-255">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="1a4c1-256">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-256">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="1a4c1-257">Batch</span><span class="sxs-lookup"><span data-stu-id="1a4c1-257">Batch</span></span>

* <span data-ttu-id="1a4c1-258">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-258">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="1a4c1-259">Cloud</span><span class="sxs-lookup"><span data-stu-id="1a4c1-259">Cloud</span></span>

* <span data-ttu-id="1a4c1-260">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-260">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="1a4c1-261">Nutzung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-261">Consumption</span></span>

* <span data-ttu-id="1a4c1-262">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-262">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="1a4c1-263">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1a4c1-263">Event Grid</span></span>

* <span data-ttu-id="1a4c1-264">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-264">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1a4c1-265">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-265">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1a4c1-266">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-266">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="1a4c1-267">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-267">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="1a4c1-268">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-268">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="1a4c1-269">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-269">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="1a4c1-270">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-270">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="1a4c1-271">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-271">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="1a4c1-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="1a4c1-272">Interactive</span></span>

* <span data-ttu-id="1a4c1-273">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-273">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="1a4c1-274">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-274">Fixed errors on startup</span></span>
* <span data-ttu-id="1a4c1-275">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-275">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="1a4c1-276">IoT</span><span class="sxs-lookup"><span data-stu-id="1a4c1-276">IoT</span></span>

* <span data-ttu-id="1a4c1-277">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-277">Added support for device provisioning service</span></span>
* <span data-ttu-id="1a4c1-278">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-278">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="1a4c1-279">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="1a4c1-279">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-280">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-280">Monitor</span></span>

* <span data-ttu-id="1a4c1-281">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-281">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="1a4c1-282">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-282">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="1a4c1-283">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-283">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-284">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-284">Network</span></span>

* <span data-ttu-id="1a4c1-285">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-285">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="1a4c1-286">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-286">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-287">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-287">Profile</span></span>

* <span data-ttu-id="1a4c1-288">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-288">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-289">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-289">Role</span></span>

* <span data-ttu-id="1a4c1-290">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-290">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1a4c1-291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1a4c1-291">Service Fabric</span></span>

* <span data-ttu-id="1a4c1-292">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-292">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="1a4c1-293">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-293">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-294">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-294">VM</span></span>

* <span data-ttu-id="1a4c1-295">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-295">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="1a4c1-296">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-296">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="1a4c1-297">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="1a4c1-297">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="1a4c1-298">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-298">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="1a4c1-299">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-299">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="1a4c1-300">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-300">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1a4c1-301">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-301">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="1a4c1-302">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-302">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="1a4c1-303">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-303">December 19, 2017</span></span>

<span data-ttu-id="1a4c1-304">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="1a4c1-304">Version 2.0.23</span></span>

* <span data-ttu-id="1a4c1-305">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-305">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-306">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-306">Container</span></span>

* <span data-ttu-id="1a4c1-307">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-307">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-308">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-308">Network</span></span>

* <span data-ttu-id="1a4c1-309">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-309">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="1a4c1-310">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-310">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-311">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-311">Storage</span></span>

* <span data-ttu-id="1a4c1-312">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-312">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-313">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-313">VM</span></span>

* <span data-ttu-id="1a4c1-314">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-314">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="1a4c1-315">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-315">December 5, 2017</span></span>

<span data-ttu-id="1a4c1-316">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="1a4c1-316">Version 2.0.22</span></span>

* <span data-ttu-id="1a4c1-317">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-317">Removed `az component` commands.</span></span> <span data-ttu-id="1a4c1-318">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-318">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-319">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-319">Core</span></span>
* <span data-ttu-id="1a4c1-320">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-320">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="1a4c1-321">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-321">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-322">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-322">ACS</span></span>

* <span data-ttu-id="1a4c1-323">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-323">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="1a4c1-324">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-324">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="1a4c1-325">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="1a4c1-325">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="1a4c1-326">Advisor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-326">Advisor</span></span>

* <span data-ttu-id="1a4c1-327">Erste Version</span><span class="sxs-lookup"><span data-stu-id="1a4c1-327">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-328">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-328">Appservice</span></span>

* <span data-ttu-id="1a4c1-329">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-329">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="1a4c1-330">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-330">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="1a4c1-331">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-331">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="1a4c1-332">Nutzung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-332">Consumption</span></span>

* <span data-ttu-id="1a4c1-333">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-333">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-334">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-334">Container</span></span>

* <span data-ttu-id="1a4c1-335">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="1a4c1-335">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-336">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-336">Monitor</span></span>

* <span data-ttu-id="1a4c1-337">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-337">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-338">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-338">Resource</span></span>

* <span data-ttu-id="1a4c1-339">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-339">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-340">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-340">Role</span></span>

* <span data-ttu-id="1a4c1-341">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-341">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="1a4c1-342">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-342">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="1a4c1-343">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-343">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-344">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-344">SQL</span></span>

* <span data-ttu-id="1a4c1-345">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-345">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="1a4c1-346">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-346">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-347">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-347">VM</span></span>

* <span data-ttu-id="1a4c1-348">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-348">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="1a4c1-349">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-349">November 14, 2017</span></span>

<span data-ttu-id="1a4c1-350">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1a4c1-350">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1a4c1-351">ACR</span><span class="sxs-lookup"><span data-stu-id="1a4c1-351">ACR</span></span>

* <span data-ttu-id="1a4c1-352">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-352">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1a4c1-353">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-353">ACS</span></span>

* <span data-ttu-id="1a4c1-354">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-354">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1a4c1-355">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="1a4c1-355">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="1a4c1-356">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-356">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="1a4c1-357">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-357">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1a4c1-358">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-358">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-359">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-359">Appservice</span></span>

* <span data-ttu-id="1a4c1-360">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-360">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1a4c1-361">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-361">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="1a4c1-362">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-362">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="1a4c1-363">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-363">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="1a4c1-364">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-364">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1a4c1-365">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-365">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="1a4c1-366">Batch</span><span class="sxs-lookup"><span data-stu-id="1a4c1-366">Batch</span></span>

* <span data-ttu-id="1a4c1-367">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="1a4c1-367">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1a4c1-368">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1a4c1-368">Batchai</span></span>

* <span data-ttu-id="1a4c1-369">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-369">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1a4c1-370">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-370">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1a4c1-371">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-371">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="1a4c1-372">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-372">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1a4c1-373">Cloud</span><span class="sxs-lookup"><span data-stu-id="1a4c1-373">Cloud</span></span>

* <span data-ttu-id="1a4c1-374">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="1a4c1-374">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-375">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-375">Container</span></span>

* <span data-ttu-id="1a4c1-376">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-376">Added support to open multiple ports</span></span>
* <span data-ttu-id="1a4c1-377">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-377">Added container group restart policy</span></span>
* <span data-ttu-id="1a4c1-378">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-378">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1a4c1-379">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-379">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1a4c1-380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1a4c1-380">Data Lake Analytics</span></span>

* <span data-ttu-id="1a4c1-381">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-381">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1a4c1-382">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-382">Data Lake Store</span></span>

* <span data-ttu-id="1a4c1-383">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-383">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1a4c1-384">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="1a4c1-384">Extension</span></span>

* <span data-ttu-id="1a4c1-385">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-385">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1a4c1-386">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-386">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1a4c1-387">IoT</span><span class="sxs-lookup"><span data-stu-id="1a4c1-387">IoT</span></span>

* <span data-ttu-id="1a4c1-388">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-388">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-389">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-389">Monitor</span></span>

* <span data-ttu-id="1a4c1-390">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-390">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-391">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-391">Network</span></span>

* <span data-ttu-id="1a4c1-392">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-392">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1a4c1-393">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-393">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="1a4c1-394">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-394">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1a4c1-395">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-395">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="1a4c1-396">Reservations</span><span class="sxs-lookup"><span data-stu-id="1a4c1-396">Reservations</span></span>

* <span data-ttu-id="1a4c1-397">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="1a4c1-397">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-398">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-398">Resource</span></span>

* <span data-ttu-id="1a4c1-399">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-399">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-400">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-400">SQL</span></span>

* <span data-ttu-id="1a4c1-401">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-401">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-402">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-402">Storage</span></span>

* <span data-ttu-id="1a4c1-403">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-403">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1a4c1-404">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-404">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1a4c1-405">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-405">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="1a4c1-406">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-406">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="1a4c1-407">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-407">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="1a4c1-408">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-408">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="1a4c1-409">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-409">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-410">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-410">VM</span></span>

* <span data-ttu-id="1a4c1-411">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-411">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1a4c1-412">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-412">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1a4c1-413">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="1a4c1-413">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1a4c1-414">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-414">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="1a4c1-415">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-415">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="1a4c1-416">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-416">October 24, 2017</span></span>

<span data-ttu-id="1a4c1-417">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1a4c1-417">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-418">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-418">Core</span></span>

* <span data-ttu-id="1a4c1-419">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="1a4c1-419">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="1a4c1-420">ACR</span><span class="sxs-lookup"><span data-stu-id="1a4c1-420">ACR</span></span>

* <span data-ttu-id="1a4c1-421">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-421">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1a4c1-422">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-422">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1a4c1-423">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-423">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-424">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-424">ACS</span></span>

* <span data-ttu-id="1a4c1-425">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-425">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1a4c1-426">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-426">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-427">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-427">Appservice</span></span>

* <span data-ttu-id="1a4c1-428">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="1a4c1-428">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1a4c1-429">Komponente</span><span class="sxs-lookup"><span data-stu-id="1a4c1-429">Component</span></span>

* <span data-ttu-id="1a4c1-430">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-430">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-431">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-431">Monitor</span></span>

* <span data-ttu-id="1a4c1-432">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-432">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-433">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-433">Resource</span></span>

* <span data-ttu-id="1a4c1-434">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-434">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="1a4c1-435">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="1a4c1-435">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-436">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-436">VM</span></span>

* <span data-ttu-id="1a4c1-437">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-437">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="1a4c1-438">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-438">October 9, 2017</span></span>

<span data-ttu-id="1a4c1-439">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1a4c1-439">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-440">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-440">Core</span></span>

* <span data-ttu-id="1a4c1-441">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-441">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-442">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-442">Appservice</span></span>

* <span data-ttu-id="1a4c1-443">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-443">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="1a4c1-444">Batch</span><span class="sxs-lookup"><span data-stu-id="1a4c1-444">Batch</span></span>

* <span data-ttu-id="1a4c1-445">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="1a4c1-445">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1a4c1-446">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-446">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1a4c1-447">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-447">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1a4c1-448">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-448">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1a4c1-449">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1a4c1-449">Batchai</span></span>

* <span data-ttu-id="1a4c1-450">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-450">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a4c1-451">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a4c1-451">Keyvault</span></span>

* <span data-ttu-id="1a4c1-452">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-452">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1a4c1-453">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-453">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1a4c1-454">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-454">Network</span></span>

* <span data-ttu-id="1a4c1-455">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-455">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1a4c1-456">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-456">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-457">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-457">Resource</span></span>

* <span data-ttu-id="1a4c1-458">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-458">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="1a4c1-459">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-459">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1a4c1-460">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-460">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1a4c1-461">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-461">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-462">Sql</span><span class="sxs-lookup"><span data-stu-id="1a4c1-462">Sql</span></span>

* <span data-ttu-id="1a4c1-463">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-463">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1a4c1-464">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-464">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1a4c1-465">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-465">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-466">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-466">Storage</span></span>

* <span data-ttu-id="1a4c1-467">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-467">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-468">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-468">Vm</span></span>

* <span data-ttu-id="1a4c1-469">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-469">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1a4c1-470">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-470">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="1a4c1-471">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-471">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="1a4c1-472">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-472">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="1a4c1-473">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-473">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="1a4c1-474">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-474">September 22, 2017</span></span>

<span data-ttu-id="1a4c1-475">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="1a4c1-475">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-476">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-476">Resource</span></span>

* <span data-ttu-id="1a4c1-477">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-477">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1a4c1-478">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-478">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1a4c1-479">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-479">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="1a4c1-480">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-480">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-481">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-481">Network</span></span>

* <span data-ttu-id="1a4c1-482">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-482">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1a4c1-483">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-483">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="1a4c1-484">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-484">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1a4c1-485">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-485">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="1a4c1-486">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-486">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1a4c1-487">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-487">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="1a4c1-488">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-488">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-489">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-489">Storage</span></span>

* <span data-ttu-id="1a4c1-490">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-490">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1a4c1-491">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="1a4c1-491">Eventgrid</span></span>

* <span data-ttu-id="1a4c1-492">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-492">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-493">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-493">SQL</span></span>

* <span data-ttu-id="1a4c1-494">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-494">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1a4c1-495">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-495">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1a4c1-496">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-496">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a4c1-497">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a4c1-497">Keyvault</span></span>

* <span data-ttu-id="1a4c1-498">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-498">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-499">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-499">VM</span></span>

* <span data-ttu-id="1a4c1-500">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-500">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="1a4c1-501">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-501">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1a4c1-502">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-502">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="1a4c1-503">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-503">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="1a4c1-504">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-504">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="1a4c1-505">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-505">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-506">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-506">ACS</span></span>

* <span data-ttu-id="1a4c1-507">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-507">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-508">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-508">Appservice</span></span>

* <span data-ttu-id="1a4c1-509">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-509">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1a4c1-510">Sicherung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-510">Backup</span></span>

* <span data-ttu-id="1a4c1-511">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="1a4c1-511">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1a4c1-512">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-512">September 11, 2017</span></span>

<span data-ttu-id="1a4c1-513">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1a4c1-513">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1a4c1-514">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-514">Core</span></span>

* <span data-ttu-id="1a4c1-515">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-515">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1a4c1-516">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-516">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-517">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-517">Acs</span></span>

* <span data-ttu-id="1a4c1-518">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-518">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1a4c1-519">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-519">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-520">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-520">Appservice</span></span>

* <span data-ttu-id="1a4c1-521">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="1a4c1-521">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1a4c1-522">CDN</span><span class="sxs-lookup"><span data-stu-id="1a4c1-522">CDN</span></span>

* <span data-ttu-id="1a4c1-523">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-523">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="1a4c1-524">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="1a4c1-524">Extension</span></span>

* <span data-ttu-id="1a4c1-525">Erste Version.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-525">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a4c1-526">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a4c1-526">Keyvault</span></span>

* <span data-ttu-id="1a4c1-527">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="1a4c1-527">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-528">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-528">Network</span></span>

* <span data-ttu-id="1a4c1-529">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-529">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1a4c1-530">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-530">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="1a4c1-531">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-531">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="1a4c1-532">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-532">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1a4c1-533">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-533">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-534">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-534">Resource</span></span>

* <span data-ttu-id="1a4c1-535">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-535">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="1a4c1-536">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-536">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="1a4c1-537">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-537">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1a4c1-538">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="1a4c1-538">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-539">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-539">SQL</span></span>

* <span data-ttu-id="1a4c1-540">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-540">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-541">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-541">VM</span></span>

* <span data-ttu-id="1a4c1-542">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-542">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1a4c1-543">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-543">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1a4c1-544">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-544">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1a4c1-545">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-545">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1a4c1-546">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-546">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1a4c1-547">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-547">August 31, 2017</span></span>

<span data-ttu-id="1a4c1-548">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1a4c1-548">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a4c1-549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a4c1-549">Keyvault</span></span>

* <span data-ttu-id="1a4c1-550">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-550">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="1a4c1-551">Sf</span><span class="sxs-lookup"><span data-stu-id="1a4c1-551">Sf</span></span>

* <span data-ttu-id="1a4c1-552">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-552">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-553">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-553">Storage</span></span>

* <span data-ttu-id="1a4c1-554">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-554">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1a4c1-555">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="1a4c1-555">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1a4c1-556">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-556">August 28, 2017</span></span>

<span data-ttu-id="1a4c1-557">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1a4c1-557">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1a4c1-558">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-558">CLI</span></span>

* <span data-ttu-id="1a4c1-559">Rechtlichen Hinweis zu `--version` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-559">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-560">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-560">ACS</span></span>

* <span data-ttu-id="1a4c1-561">Vorschauregionen korrigiert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-561">Corrected preview regions.</span></span>
* <span data-ttu-id="1a4c1-562">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-562">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="1a4c1-563">ACS-Befehlsausgabe optimiert.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-563">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-564">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-564">Appservice</span></span>

* <span data-ttu-id="1a4c1-565">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-565">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="1a4c1-566">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-566">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="1a4c1-567">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-567">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="1a4c1-568">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-568">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1a4c1-569">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-569">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1a4c1-570">IoT</span><span class="sxs-lookup"><span data-stu-id="1a4c1-570">IoT</span></span>

* <span data-ttu-id="1a4c1-571">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="1a4c1-571">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-572">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-572">Network</span></span>

* <span data-ttu-id="1a4c1-573">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-573">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1a4c1-574">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `vnet subnet [create|update]` in `--service-endpoints` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-574">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="1a4c1-575">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-575">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1a4c1-576">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-576">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1a4c1-577">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-577">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-578">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-578">Profile</span></span>

* <span data-ttu-id="1a4c1-579">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-579">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1a4c1-580">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1a4c1-580">Service Fabric</span></span>

* <span data-ttu-id="1a4c1-581">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="1a4c1-581">Preview release</span></span>
* <span data-ttu-id="1a4c1-582">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-582">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1a4c1-583">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-583">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1a4c1-584">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-584">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-585">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-585">Storage</span></span>

* <span data-ttu-id="1a4c1-586">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-586">Enabled setting blob tier</span></span>
* <span data-ttu-id="1a4c1-587">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-587">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1a4c1-588">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-588">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="1a4c1-589">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-589">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1a4c1-590">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-590">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1a4c1-591">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-591">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-592">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-592">VM</span></span>

* <span data-ttu-id="1a4c1-593">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-593">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="1a4c1-594">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-594">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="1a4c1-595">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-595">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="1a4c1-596">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-596">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1a4c1-597">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-597">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1a4c1-598">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-598">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="1a4c1-599">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-599">August 15, 2017</span></span>

<span data-ttu-id="1a4c1-600">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1a4c1-600">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-601">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-601">ACS</span></span>

* <span data-ttu-id="1a4c1-602">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-602">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-603">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-603">Appservice</span></span>

* <span data-ttu-id="1a4c1-604">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-604">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1a4c1-605">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1a4c1-605">Event Grid</span></span>

* <span data-ttu-id="1a4c1-606">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-606">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1a4c1-607">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-607">August 11, 2017</span></span>

<span data-ttu-id="1a4c1-608">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1a4c1-608">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-609">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-609">ACS</span></span>

* <span data-ttu-id="1a4c1-610">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-610">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1a4c1-611">Batch</span><span class="sxs-lookup"><span data-stu-id="1a4c1-611">Batch</span></span>

* <span data-ttu-id="1a4c1-612">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-612">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1a4c1-613">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-613">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1a4c1-614">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-614">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1a4c1-615">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-615">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1a4c1-616">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="1a4c1-616">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1a4c1-617">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-617">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1a4c1-618">Komponente</span><span class="sxs-lookup"><span data-stu-id="1a4c1-618">Component</span></span>

* <span data-ttu-id="1a4c1-619">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-619">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1a4c1-620">Container</span><span class="sxs-lookup"><span data-stu-id="1a4c1-620">Container</span></span>

* <span data-ttu-id="1a4c1-621">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="1a4c1-621">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1a4c1-622">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-622">Data Lake Store</span></span>

* <span data-ttu-id="1a4c1-623">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-623">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1a4c1-624">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1a4c1-624">Event Grid</span></span>

* <span data-ttu-id="1a4c1-625">Erste Version</span><span class="sxs-lookup"><span data-stu-id="1a4c1-625">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-626">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-626">Network</span></span>

* <span data-ttu-id="1a4c1-627">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-627">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="1a4c1-628">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="1a4c1-628">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="1a4c1-629">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-629">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1a4c1-630">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-630">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-631">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-631">Profile</span></span>

* <span data-ttu-id="1a4c1-632">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="1a4c1-632">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-633">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-633">Storage</span></span>

* <span data-ttu-id="1a4c1-634">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-634">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-635">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-635">VM</span></span>

* <span data-ttu-id="1a4c1-636">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-636">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1a4c1-637">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-637">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1a4c1-638">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-638">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1a4c1-639">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="1a4c1-639">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1a4c1-640">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-640">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1a4c1-641">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-641">July 28, 2017</span></span>

<span data-ttu-id="1a4c1-642">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1a4c1-642">Version 2.0.12</span></span>

* <span data-ttu-id="1a4c1-643">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-643">Added container commands</span></span>
* <span data-ttu-id="1a4c1-644">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-644">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1a4c1-645">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-645">Core</span></span>

* <span data-ttu-id="1a4c1-646">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-646">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1a4c1-647">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-647">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1a4c1-648">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="1a4c1-648">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1a4c1-649">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-649">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1a4c1-650">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-650">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1a4c1-651">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-651">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1a4c1-652">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-652">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1a4c1-653">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-653">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1a4c1-654">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-654">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1a4c1-655">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-655">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1a4c1-656">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="1a4c1-656">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1a4c1-657">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-657">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1a4c1-658">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-658">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1a4c1-659">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-659">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1a4c1-660">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1a4c1-660">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1a4c1-661">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-661">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1a4c1-662">ACR</span><span class="sxs-lookup"><span data-stu-id="1a4c1-662">ACR</span></span>

* <span data-ttu-id="1a4c1-663">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-663">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1a4c1-664">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-664">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1a4c1-665">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-665">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1a4c1-666">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-666">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1a4c1-667">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-667">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1a4c1-668">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-668">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-669">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-669">ACS</span></span>

* <span data-ttu-id="1a4c1-670">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="1a4c1-670">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-671">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-671">Appservice</span></span>

* <span data-ttu-id="1a4c1-672">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-672">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1a4c1-673">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="1a4c1-673">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1a4c1-674">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-674">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="1a4c1-675">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-675">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1a4c1-676">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-676">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1a4c1-677">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-677">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1a4c1-678">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-678">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1a4c1-679">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-679">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1a4c1-680">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-680">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1a4c1-681">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-681">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="1a4c1-682">Batch</span><span class="sxs-lookup"><span data-stu-id="1a4c1-682">Batch</span></span>

* <span data-ttu-id="1a4c1-683">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-683">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1a4c1-684">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-684">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="1a4c1-685">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-685">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="1a4c1-686">CDN</span><span class="sxs-lookup"><span data-stu-id="1a4c1-686">CDN</span></span>

* <span data-ttu-id="1a4c1-687">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="1a4c1-687">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="1a4c1-688">Cloud</span><span class="sxs-lookup"><span data-stu-id="1a4c1-688">Cloud</span></span>

* <span data-ttu-id="1a4c1-689">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-689">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1a4c1-690">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a4c1-690">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1a4c1-691">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-691">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1a4c1-692">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="1a4c1-692">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1a4c1-693">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-693">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1a4c1-694">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1a4c1-694">CosmosDB</span></span>

* <span data-ttu-id="1a4c1-695">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-695">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1a4c1-696">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-696">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1a4c1-697">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1a4c1-697">Data Lake Analytics</span></span>

* <span data-ttu-id="1a4c1-698">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-698">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1a4c1-699">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-699">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="1a4c1-700">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-700">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1a4c1-701">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-701">Data Lake Store</span></span>

* <span data-ttu-id="1a4c1-702">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-702">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="1a4c1-703">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="1a4c1-703">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1a4c1-704">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-704">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1a4c1-705">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-705">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1a4c1-706">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="1a4c1-706">Interactive</span></span>

* <span data-ttu-id="1a4c1-707">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-707">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1a4c1-708">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-708">Increased test coverage</span></span>
* <span data-ttu-id="1a4c1-709">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-709">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1a4c1-710">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-710">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1a4c1-711">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-711">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1a4c1-712">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-712">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1a4c1-713">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-713">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1a4c1-714">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-714">Added `--progress` flag</span></span>
* <span data-ttu-id="1a4c1-715">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-715">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1a4c1-716">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-716">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1a4c1-717">IoT</span><span class="sxs-lookup"><span data-stu-id="1a4c1-717">IoT</span></span>

* <span data-ttu-id="1a4c1-718">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="1a4c1-718">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1a4c1-719">(3934)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-719">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1a4c1-720">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-720">Key vault</span></span>

* <span data-ttu-id="1a4c1-721">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-721">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="1a4c1-722">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-722">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="1a4c1-723">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-723">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1a4c1-724">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-724">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1a4c1-725">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-725">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="1a4c1-726">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-726">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1a4c1-727">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-727">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1a4c1-728">(3307)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-728">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1a4c1-729">Labor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-729">Lab</span></span>

* <span data-ttu-id="1a4c1-730">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-730">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="1a4c1-731">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-731">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-732">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-732">Monitor</span></span>

* <span data-ttu-id="1a4c1-733">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-733">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1a4c1-734">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-734">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="1a4c1-735">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-735">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="1a4c1-736">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-736">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="1a4c1-737">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-737">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="1a4c1-738">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-738">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="1a4c1-739">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-739">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1a4c1-740">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-740">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="1a4c1-741">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a4c1-741">`location` no longer required</span></span>
  * <span data-ttu-id="1a4c1-742">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="1a4c1-742">Add name and ID support for target</span></span>
  * <span data-ttu-id="1a4c1-743">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-743">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="1a4c1-744">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-744">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="1a4c1-745">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-745">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1a4c1-746">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="1a4c1-746">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1a4c1-747">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-747">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1a4c1-748">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-748">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-749">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-749">Network</span></span>

* <span data-ttu-id="1a4c1-750">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-750">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1a4c1-751">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-751">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="1a4c1-752">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-752">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1a4c1-753">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-753">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1a4c1-754">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="1a4c1-754">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="1a4c1-755">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-755">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1a4c1-756">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-756">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="1a4c1-757">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-757">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="1a4c1-758">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-758">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1a4c1-759">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-759">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="1a4c1-760">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-760">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="1a4c1-761">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-761">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="1a4c1-762">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-762">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="1a4c1-763">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-763">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="1a4c1-764">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-764">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="1a4c1-765">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-765">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="1a4c1-766">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-766">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1a4c1-767">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="1a4c1-767">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="1a4c1-768">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-768">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="1a4c1-769">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-769">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="1a4c1-770">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-770">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="1a4c1-771">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-771">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1a4c1-772">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-772">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="1a4c1-773">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-773">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1a4c1-774">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-774">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1a4c1-775">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-775">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1a4c1-776">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-776">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-777">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-777">Profile</span></span>

* <span data-ttu-id="1a4c1-778">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="1a4c1-778">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1a4c1-779">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="1a4c1-779">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1a4c1-780">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-780">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1a4c1-781">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-781">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1a4c1-782">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="1a4c1-782">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1a4c1-783">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-783">RDBMS</span></span>

* <span data-ttu-id="1a4c1-784">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-784">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1a4c1-785">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-785">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1a4c1-786">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-786">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1a4c1-787">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-787">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-788">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-788">Resource</span></span>

* <span data-ttu-id="1a4c1-789">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-789">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="1a4c1-790">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="1a4c1-790">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1a4c1-791">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-791">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1a4c1-792">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-792">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1a4c1-793">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-793">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1a4c1-794">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-794">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="1a4c1-795">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-795">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1a4c1-796">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-796">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-797">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-797">Role</span></span>

* <span data-ttu-id="1a4c1-798">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-798">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="1a4c1-799">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-799">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1a4c1-800">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="1a4c1-800">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1a4c1-801">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-801">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="1a4c1-802">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-802">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1a4c1-803">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1a4c1-803">Service Fabric</span></span>
* <span data-ttu-id="1a4c1-804">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-804">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1a4c1-805">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-805">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1a4c1-806">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-806">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-807">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-807">SQL</span></span>

* <span data-ttu-id="1a4c1-808">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-808">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1a4c1-809">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-809">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1a4c1-810">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-810">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-811">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-811">Storage</span></span>

* <span data-ttu-id="1a4c1-812">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-812">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1a4c1-813">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-813">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1a4c1-814">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-814">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1a4c1-815">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-815">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="1a4c1-816">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-816">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="1a4c1-817">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-817">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-818">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-818">VM</span></span>

* <span data-ttu-id="1a4c1-819">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="1a4c1-819">Support configuring nsg</span></span>
* <span data-ttu-id="1a4c1-820">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="1a4c1-820">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1a4c1-821">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-821">Support managed service identities</span></span>
* <span data-ttu-id="1a4c1-822">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-822">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="1a4c1-823">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-823">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1a4c1-824">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-824">May 10, 2017</span></span>

<span data-ttu-id="1a4c1-825">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1a4c1-825">Version 2.0.6</span></span>

* <span data-ttu-id="1a4c1-826">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-826">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1a4c1-827">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-827">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1a4c1-828">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="1a4c1-828">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="1a4c1-829">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-829">Include Cognitive Services module.</span></span>
* <span data-ttu-id="1a4c1-830">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-830">Include Service Fabric module.</span></span>
* <span data-ttu-id="1a4c1-831">Einbeziehen des interaktiven Moduls (Umbenennen von az-shell)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-831">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="1a4c1-832">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-832">Add support for CDN commands.</span></span>
* <span data-ttu-id="1a4c1-833">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-833">Remove Container module.</span></span>
* <span data-ttu-id="1a4c1-834">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-834">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1a4c1-835">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-835">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1a4c1-836">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-836">Core</span></span>

* <span data-ttu-id="1a4c1-837">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-837">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="1a4c1-838">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-838">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1a4c1-839">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-839">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1a4c1-840">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-840">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1a4c1-841">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-841">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1a4c1-842">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-842">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1a4c1-843">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-843">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1a4c1-844">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-844">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1a4c1-845">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-845">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1a4c1-846">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-846">core: Improved performance</span></span>
* <span data-ttu-id="1a4c1-847">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-847">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1a4c1-848">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="1a4c1-848">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-849">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-849">ACS</span></span>

* <span data-ttu-id="1a4c1-850">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a4c1-850">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1a4c1-851">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-851">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1a4c1-852">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-852">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1a4c1-853">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-853">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-854">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-854">AppService</span></span>

* <span data-ttu-id="1a4c1-855">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-855">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1a4c1-856">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-856">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1a4c1-857">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-857">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1a4c1-858">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="1a4c1-858">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1a4c1-859">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-859">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1a4c1-860">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-860">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1a4c1-861">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="1a4c1-861">support slot swap with preview</span></span>
* <span data-ttu-id="1a4c1-862">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-862">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1a4c1-863">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-863">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1a4c1-864">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1a4c1-864">CosmosDB</span></span>

* <span data-ttu-id="1a4c1-865">Umbenennen des documentdb-Moduls in cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-865">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="1a4c1-866">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-866">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1a4c1-867">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-867">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1a4c1-868">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="1a4c1-868">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1a4c1-869">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1a4c1-869">Data Lake Analytics</span></span>

* <span data-ttu-id="1a4c1-870">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="1a4c1-870">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="1a4c1-871">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-871">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1a4c1-872">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-872">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="1a4c1-873">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="1a4c1-873">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1a4c1-874">Table</span><span class="sxs-lookup"><span data-stu-id="1a4c1-874">Table</span></span>
  * <span data-ttu-id="1a4c1-875">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="1a4c1-875">Table valued function</span></span>
  * <span data-ttu-id="1a4c1-876">Sicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-876">View</span></span>
  * <span data-ttu-id="1a4c1-877">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-877">Table Statistics.</span></span> <span data-ttu-id="1a4c1-878">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-878">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1a4c1-879">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-879">Data Lake Store</span></span>

* <span data-ttu-id="1a4c1-880">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-880">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="1a4c1-881">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-881">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1a4c1-882">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="1a4c1-882">missed help for access show.</span></span> <span data-ttu-id="1a4c1-883">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="1a4c1-883">adding it.</span></span> <span data-ttu-id="1a4c1-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1a4c1-885">Suchen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-885">Find</span></span>

* <span data-ttu-id="1a4c1-886">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="1a4c1-886">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a4c1-887">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a4c1-887">KeyVault</span></span>

* <span data-ttu-id="1a4c1-888">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-888">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1a4c1-889">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-889">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="1a4c1-890">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="1a4c1-890">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1a4c1-891">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="1a4c1-891">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="1a4c1-892">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-892">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1a4c1-893">Labor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-893">Lab</span></span>

* <span data-ttu-id="1a4c1-894">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="1a4c1-894">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="1a4c1-895">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-895">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="1a4c1-896">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="1a4c1-896">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="1a4c1-897">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="1a4c1-897">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="1a4c1-898">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="1a4c1-898">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="1a4c1-899">Überwachen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-899">Monitor</span></span>

* <span data-ttu-id="1a4c1-900">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-900">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1a4c1-901">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-901">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1a4c1-902">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-902">Network</span></span>

* <span data-ttu-id="1a4c1-903">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-903">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="1a4c1-904">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-904">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="1a4c1-905">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="1a4c1-905">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="1a4c1-906">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-906">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="1a4c1-907">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="1a4c1-907">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="1a4c1-908">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="1a4c1-908">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="1a4c1-909">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-909">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="1a4c1-910">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-910">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="1a4c1-911">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-911">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="1a4c1-912">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="1a4c1-912">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1a4c1-913">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-913">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="1a4c1-914">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-914">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="1a4c1-915">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="1a4c1-915">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="1a4c1-916">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="1a4c1-916">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="1a4c1-917">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="1a4c1-917">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="1a4c1-918">Hinzufügen von „network watcher“-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-918">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="1a4c1-919">Profil</span><span class="sxs-lookup"><span data-stu-id="1a4c1-919">Profile</span></span>

* <span data-ttu-id="1a4c1-920">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-920">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1a4c1-921">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-921">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1a4c1-922">Redis</span><span class="sxs-lookup"><span data-stu-id="1a4c1-922">Redis</span></span>

* <span data-ttu-id="1a4c1-923">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-923">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1a4c1-924">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-924">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="1a4c1-925">Ressource</span><span class="sxs-lookup"><span data-stu-id="1a4c1-925">Resource</span></span>

* <span data-ttu-id="1a4c1-926">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-926">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1a4c1-927">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-927">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1a4c1-928">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-928">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1a4c1-929">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="1a4c1-929">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1a4c1-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1a4c1-931">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-931">Add docs for az lock update.</span></span> <span data-ttu-id="1a4c1-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1a4c1-933">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-933">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1a4c1-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1a4c1-935">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="1a4c1-935">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1a4c1-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1a4c1-937">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-937">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1a4c1-938">Rolle</span><span class="sxs-lookup"><span data-stu-id="1a4c1-938">Role</span></span>

* <span data-ttu-id="1a4c1-939">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-939">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1a4c1-940">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-940">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1a4c1-941">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-941">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1a4c1-942">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="1a4c1-942">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1a4c1-943">SQL</span><span class="sxs-lookup"><span data-stu-id="1a4c1-943">SQL</span></span>

* <span data-ttu-id="1a4c1-944">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-944">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="1a4c1-945">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-945">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1a4c1-946">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-946">Storage</span></span>

* <span data-ttu-id="1a4c1-947">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-947">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="1a4c1-948">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="1a4c1-948">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1a4c1-949">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="1a4c1-949">Add support for large block blob upload</span></span>
* <span data-ttu-id="1a4c1-950">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="1a4c1-950">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-951">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-951">VM</span></span>

* <span data-ttu-id="1a4c1-952">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="1a4c1-952">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1a4c1-953">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-953">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1a4c1-954">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1a4c1-954">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1a4c1-955">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-955">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1a4c1-956">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-956">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1a4c1-957">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="1a4c1-957">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1a4c1-958">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-958">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1a4c1-959">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-959">April 3, 2017</span></span>

<span data-ttu-id="1a4c1-960">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1a4c1-960">Version 2.0.2</span></span>

<span data-ttu-id="1a4c1-961">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-961">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="1a4c1-962">Core</span><span class="sxs-lookup"><span data-stu-id="1a4c1-962">Core</span></span>

* <span data-ttu-id="1a4c1-963">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="1a4c1-963">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="1a4c1-964">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-964">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1a4c1-965">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-965">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1a4c1-966">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-966">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1a4c1-967">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-967">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1a4c1-968">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="1a4c1-968">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1a4c1-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1a4c1-970">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-970">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1a4c1-971">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="1a4c1-971">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="1a4c1-972">ACS</span><span class="sxs-lookup"><span data-stu-id="1a4c1-972">ACS</span></span>

* <span data-ttu-id="1a4c1-973">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-973">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1a4c1-974">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="1a4c1-974">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1a4c1-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1a4c1-976">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="1a4c1-976">Add support for windows clusters.</span></span> <span data-ttu-id="1a4c1-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1a4c1-978">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="1a4c1-978">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1a4c1-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="1a4c1-980">AppService</span><span class="sxs-lookup"><span data-stu-id="1a4c1-980">AppService</span></span>

* <span data-ttu-id="1a4c1-981">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-981">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1a4c1-982">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-982">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1a4c1-983">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-983">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1a4c1-984">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-984">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="1a4c1-985">DataLake</span><span class="sxs-lookup"><span data-stu-id="1a4c1-985">DataLake</span></span>

* <span data-ttu-id="1a4c1-986">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-986">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="1a4c1-987">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="1a4c1-987">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="1a4c1-988">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="1a4c1-988">DocuemntDB</span></span>

* <span data-ttu-id="1a4c1-989">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-989">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1a4c1-990">VM</span><span class="sxs-lookup"><span data-stu-id="1a4c1-990">VM</span></span>

* <span data-ttu-id="1a4c1-991">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-991">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1a4c1-992">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-992">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1a4c1-993">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-993">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1a4c1-994">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-994">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1a4c1-995">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-995">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1a4c1-996">Hinzufügen von „--secrets“ für VM und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-996">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="1a4c1-997">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="1a4c1-997">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1a4c1-998">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="1a4c1-998">February 27, 2017</span></span>

<span data-ttu-id="1a4c1-999">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1a4c1-999">Version 2.0.0</span></span>

<span data-ttu-id="1a4c1-1000">Diese Version von Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1000">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="1a4c1-1001">Die allgemeine Verfügbarkeit gilt für diese Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1001">General availability applies to these command modules:</span></span>
- <span data-ttu-id="1a4c1-1002">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1002">Container Service (acs)</span></span>
- <span data-ttu-id="1a4c1-1003">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1003">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1a4c1-1004">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1004">Networking</span></span>
- <span data-ttu-id="1a4c1-1005">Speicher</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1005">Storage</span></span>

<span data-ttu-id="1a4c1-1006">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1006">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="1a4c1-1007">Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1007">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="1a4c1-1008">Sie haben die Möglichkeit, Fragen in [Stack Overflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1008">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="1a4c1-1009">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure-CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1009">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="1a4c1-1010">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1010">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="1a4c1-1011">In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1011">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="1a4c1-1012">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1012">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="1a4c1-1013">Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1013">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="1a4c1-1014">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1014">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="1a4c1-1015">Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1015">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="1a4c1-1016">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1016">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1a4c1-1017">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1017">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1a4c1-1018">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1018">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="1a4c1-1019">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="1a4c1-1019">Provide feedback from the command line with the `az feedback` command.</span></span>

