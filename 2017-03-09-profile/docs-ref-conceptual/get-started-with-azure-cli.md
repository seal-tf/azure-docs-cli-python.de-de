---
title: Erste Schritte mit Azure CLI 2.0
description: "Enthält eine Beschreibung der ersten Schritte mit Azure CLI 2.0 unter Linux, MacOS und Windows."
keywords: Azure CLI 2.0, Linux, MacOS, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 11153c13fb9868897b0bb21dac9d64072c3af16e
ms.sourcegitcommit: 70c4d7a14591e5b761e261105cd2d376753f2a54
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/19/2017
---
# <a name="get-started-with-azure-cli-20"></a>Erste Schritte mit Azure CLI 2.0

Azure CLI 2.0 ist die neue Befehlszeilenumgebung von Azure und dient zum Verwalten von Azure-Ressourcen.
Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux und Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.

Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert.
Dieser Artikel hilft Ihnen beim Einstieg und enthält Informationen zu den wichtigsten Konzepten.

Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).

## <a name="connect"></a>Verbinden

Die einfachste Möglichkeit, erste Schritte auszuführen, besteht im [Starten von Cloud Shell](/azure/cloud-shell/quickstart).

1. Starten Sie Cloud Shell über den oberen Navigationsbereich im Azure-Portal.

   ![Shell-Symbol](media/get-started-with-azure-cli/shell-icon.png)

2. Wählen Sie das zu verwendende Abonnement aus, und erstellen Sie ein Speicherkonto.

   ![Erstellen Sie ein Speicherkonto.](media/get-started-with-azure-cli/storage-prompt.png)

Sie können die CLI auch [installieren](install-azure-cli.md) und lokal über die Befehlszeile ausführen. Führen Sie nach der Installation der CLI `az login` aus, um sich mit Ihrem Standardabonnement anzumelden.

## <a name="create-a-resource-group"></a>Erstellen einer Ressourcengruppe

Nachdem nun alles eingerichtet ist, können wir mit der Azure-CLI Ressourcen in Azure erstellen.

Erstellen Sie zunächst eine Ressourcengruppe.  Ressourcengruppen ermöglichen in Azure die Verwaltung mehrerer Ressourcen, die Sie zu einer logischen Gruppe zusammenfassen möchten.  So können Sie etwa eine Ressourcengruppe für eine Anwendung oder für ein Projekt erstellen und darin einen virtuellen Computer, eine Datenbank und einen CDN-Dienst hinzufügen.

Hier erstellen wir eine Ressourcengruppe namens „MyResourceGroup“ in der Azure-Region *westus2*.  Geben Sie hierzu folgenden Befehl ein:

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

Nachdem die Ressourcengruppe erstellt wurde, werden mit dem Befehl `az group create` mehrere Eigenschaften der neu erstellten Ressource ausgegeben:

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a>Erstellen eines virtuellen Linux-Computers

Nachdem wir nun über eine Ressourcengruppe verfügen, erstellen wir darin einen virtuellen Linux-Computer.

Sie können einen virtuellen Linux-Computer mithilfe des beliebten UbuntuLTS-Images mit zwei angefügten Speicherdatenträgern der Größe 10 GB und 20 GB erstellen, indem Sie den folgenden Befehl verwenden:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

Wenn Sie den obigen Befehl ausführen, sucht Azure CLI 2.0 im Verzeichnis „~/.ssh“ nach einem gespeicherten SSH-Schlüsselpaar.  Falls Sie an diesem Speicherort nicht bereits ein SSH-Schlüsselpaar gespeichert haben, können Sie es von der Azure-CLI automatisch erstellen lassen. Übergeben Sie hierzu den Parameter „--generate-ssh-keys“:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

Mit dem Befehl `az vm create` wird die Ausgabe durchgeführt, nachdem die VM vollständig erstellt wurde und bereit für den Zugriff und die Nutzung ist. Die Ausgabe umfasst mehrere Eigenschaften der neu erstellten VM, z.B. deren öffentliche IP-Adresse:

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

Nach Erstellung des virtuellen Computers können Sie sich bei Ihrem neuen virtuellen Linux-Computer anmelden. Verwenden Sie hierzu **SSH** und die öffentliche IP-Adresse des virtuellen Computers, den Sie erstellt haben:

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a>Erstellen eines virtuellen Windows Server-Computers

Als Nächstes erstellen wir eine VM basierend auf Windows Server 2016 Datacenter, indem wir den Befehl `az vm create` verwenden und die VM derselben Ressourcengruppe namens „MyResourceGroup“ hinzufügen, die wir für die Linux-VM genutzt haben.  Wie im Beispiel für die Linux-VM auch, fügen wir mit dem Parameter `--data-disk-sizes-gb` zwei Speicherdatenträger hinzu.

Für Azure ist es erforderlich, dass Sie die Verwendung von Benutzernamen und Kennwörtern vermeiden, die leicht erraten werden können. Es gelten bestimmte Regeln, welche Zeichen zulässig sind, und auch die Mindestlänge von Benutzername und Kennwort ist vorgegeben.  

> [!NOTE]
> Beim Ausführen dieses Befehls werden Sie aufgefordert, Ihren Benutzernamen und Ihr Kennwort einzugeben.

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

Der Befehl `az vm create` gibt Ergebnisse aus, wenn der virtuelle Computer vollständig erstellt wurde und einsatzbereit ist.

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

Melden Sie sich nun unter Verwendung von Remotedesktop und der öffentlichen IP-Adresse des virtuellen Computers (wird in der Ausgabe von `az vm create` zurückgegeben) bei Ihrem neu erstellten virtuellen Windows Server-Computer an.  
Bei einem Windows-basierten System können Sie hierzu über die Befehlszeile den Befehl `mstsc` ausführen:

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

Geben Sie bei der Anmeldung die gleiche Kombination aus Benutzername und Kennwort an, die Sie auch beim Erstellen des virtuellen Computers verwendet haben.

## <a name="creating-other-resources-in-azure"></a>Erstellen anderer Ressourcen in Azure

Sie wissen nun, wie Sie eine Ressourcengruppe, einen virtuellen Linux-Computer und einen virtuellen Windows Server-Computer erstellen. Sie können aber auch noch viele andere Arten von Azure-Ressourcen erstellen.  

Alle neuen Ressourcen werden mit dem einheitlichen Benennungsmuster `az <resource type name> create` erstellt.  Mithilfe des folgenden create-Befehls können Sie beispielsweise einen Azure-Netzwerklastenausgleich erstellen, den wir dann unseren neu erstellten virtuellen Computern zuordnen können:

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

Wir könnten für unsere Infrastruktur auch ein neues privates virtuelles Netzwerk (in Azure für gewöhnlich als VNET bezeichnet) erstellen. Hierfür wird der folgende create-Befehl verwendet:

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

Das Praktische an Azure und der Azure-CLI ist, dass wir damit nicht nur eine cloudbasierte Infrastruktur erhalten, sondern auch verwaltete Plattformdienste erstellen können.  Die verwalteten Plattformdienste lassen sich zudem mit Infrastrukturelementen zu noch leistungsfähigeren Lösungen kombinieren.

So können Sie beispielsweise mithilfe der Azure-CLI eine Azure App Service-Instanz erstellen.  Azure App Service ist ein verwalteter Plattformdienst, der sich bestens zum Hosten von Web-Apps eignet, ohne dass Sie sich dabei Gedanken um die Infrastruktur machen müssen.  Nach der Erstellung der Azure App Service-Instanz können Sie darin mithilfe der folgenden create-Befehle zwei neue Azure-Web-Apps erstellen:

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

Wenn Sie die Funktionsweise des Musters `az <resource type name> create` verstanden haben, ist die Erstellung von Elementen sehr einfach. Hier sind einige gängige Azure-Ressourcentypen und die entsprechenden Erstellungsbefehle der Azure-CLI angegeben:

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

Die [Referenzdokumentation](/cli/azure) enthält weitere Informationen zu ressourcenspezifischen Parametern, die Sie an die obigen Befehle übergeben können, und zu den verfügbaren Ressourcentypen. 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>Nützlicher Tipp: Optimieren von Erstellungsvorgängen mit „--no-wait“

Beim Erstellen von Ressourcen per Azure CLI 2.0 wird beim Befehl `az <resource type name> create` standardmäßig gewartet, bis die Ressource erstellt wurde und bereit für die Nutzung ist.  Wenn Sie beispielsweise eine VM erstellen, wird die Rückgabe für den Befehl `az vm create` standardmäßig erst durchgeführt, nachdem die VM erstellt wurde und bereit für die SSH- bzw. RDP-Verbindung ist.

Der Grund für diesen Ansatz ist, dass so das Schreiben von Automatisierungsskripts vereinfacht wird, die mehrere Schritte mit Abhängigkeiten enthalten (und die erfolgreiche Durchführung einer vorgeschalteten Aufgabe erfordern, bevor fortgefahren werden kann).

Falls Sie vor dem Fortfahren nicht auf die Erstellung einer Ressource warten müssen, können Sie die Option `no-wait` verwenden, um im Hintergrund eine Erstellungsaktion zu starten. Sie können die CLI für andere Befehle weiterverwenden.

Bei der folgenden Nutzung von `az vm create` wird eine VM-Bereitstellung gestartet und die Rückgabe dann deutlich schneller durchgeführt (vor dem vollständigen Starten der VM):

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

Der Einsatz von `--no-wait` kann bei der erheblichen Optimierung der Leistung Ihrer Automatisierungsskripts hilfreich sein.

## <a name="listing-resources-and-formatting-output"></a>Auflisten von Ressourcen und Formatieren der Ausgabe

Sie können den Befehl `list` in der Azure-CLI verwenden, um die in Azure ausgeführten Ressourcen zu ermitteln und aufzulisten. 

Wie mit dem create-Befehl auch, können Sie Ressourcen per Azure CLI 2.0 auflisten, indem Sie das gängige Benennungsmuster `az <resource type name> list` verwenden, das für alle Ressourcentypen einheitlich ist.  Es sind verschiedene Ausgabeformate und Abfrageoptionen verfügbar, um die Liste mit den Ressourcen auf die gewünschte Weise zu filtern und zu sortieren.

Mit `az vm list` wird beispielsweise die Liste mit allen vorhandenen VMs angezeigt.   

```azurecli-interactive
az vm list 
```
Die zurückgegebenen Werte liegen standardmäßig im JSON-Format vor (aus Platzgründen nur eine Teilausgabe).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...   
]
```

Sie können das Ausgabeformat mit der Option `--output` optional ändern.  Führen Sie den Befehl `az vm list` aus, um die zuvor erstellten Linux- und Windows Server-VMs sowie die am häufigsten verwendeten Eigenschaften einer VM anzuzeigen, indem Sie die leicht lesbare Formatoption *table* nutzen:

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Sie können die Ausgabeoption *tsv* verwenden, um ein textbasiertes Format mit Tabulatortrennung und ohne Überschriften zu erhalten.  Dieses Format ist nützlich, wenn Sie die Ausgabe an ein anderes textbasiertes Tool wie beispielsweise grep senden möchten. 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
Der Artikel zu den [Ausgabeformaten](format-output-azure-cli.md) enthält Informationen zu weiteren Möglichkeiten zum Auflisten von Ressourcen und Formatieren der Ausgabe.

## <a name="querying-resources-and-shaping-outputs"></a>Abfragen von Ressourcen und Formen von Ausgaben

Es kann häufiger vorkommen, dass Sie nur nach den Ressourcen suchen möchten, die einen bestimmte Bedingung erfüllen.  

Der Befehl `list` verfügt über eine integrierte Unterstützung von Funktionen, die das Filtern von Ressourcen nach dem Namen der Ressourcengruppe einfach machen.  Beispielsweise können Sie den Parameter `--ResourceGroup` oder `-g` an den Befehl `list` übergeben, um nur die Ressourcen einer bestimmten Ressourcengruppe abzurufen:


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Zur noch besseren Unterstützung von Abfragen können Sie den Parameter `--query` verwenden, um für die Ergebnisse *jedes* `az`-Befehls eine JMESPath-Abfrage durchzuführen.  Mit JMESPath-Abfragen kann die Ausgabe aller zurückgegebenen Ergebnisse sowohl gefiltert als auch geformt werden.

Führen Sie beispielsweise den folgenden Befehl aus, um eine Abfrage für alle VM-Ressourcen in Ressourcengruppen durchzuführen, die „My“ enthalten:

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Anschließend können wir die Ausgabe weiter verfeinern, indem wir die Formungsfunktion von JMESPath-Abfragen zum zusätzlichen Ausgeben von unterschiedlichen Werten verwenden.  Mit dem folgenden Befehl wird beispielsweise der Typ des Betriebssystemdatenträgers abgerufen, über den die VM ermitteln kann, ob ein Linux- oder Windows-basiertes Betriebssystem verwendet wird:

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

Die JMESPath-Unterstützung in der Azure-CLI ist sehr leistungsstark.  Weitere Informationen zur Verwendung finden Sie im Artikel zu [Abfragen](query-azure-cli.md).

## <a name="deleting-resources"></a>Löschen von Ressourcen

Sie können den Befehl `delete` in der Azure-CLI nutzen, um nicht mehr benötigte Ressourcen zu löschen. Sie können den Befehl `delete` – wie auch beim Befehl `create` – mit einer beliebigen Ressource verwenden.

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

Standardmäßig zeigt die CLI eine Aufforderung zum Bestätigen des Löschvorgangs an.  Sie können diese Aufforderung für automatisierte Skripts unterdrücken.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

Außerdem können Sie den Befehl `delete` nutzen, um mehrere Ressourcen gleichzeitig zu löschen. Der folgende Befehl löscht beispielsweise alle Ressourcen der Ressourcengruppe „MyResourceGroup“, die wir in den Beispielen dieses Tutorials verwendet haben.

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>Herunterladen von Beispielen

Weitere Informationen zu den Verwendungsmöglichkeiten der Azure-CLI finden Sie in unseren allgemeinen Skripts für [virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web-Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) und [SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).

## <a name="read-the-api-reference-docs"></a>Lesen Sie die API-Referenzdokumente

[API-Referenz](/cli/azure)

## <a name="get-help"></a>Hier erhalten Sie Hilfe

Die Azure-CLI verfügt über eine integrierte Hilfedokumentation, die unserer Webdokumentation entspricht. Sie können sie über die Befehlszeile ausführen:

```azurecli-interactive
az [command-group [command]] -h
```

Verwenden Sie beispielsweise Folgendes, um anzuzeigen, welche Befehle und Untergruppen für VMs verfügbar sind:

```azurecli-interactive
az vm -h
```

Verwenden Sie Folgendes, um Hilfe zum Befehl für die Erstellung einer VM zu erhalten:

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Durchführen der Umstellung von Azure CLI 1.0

Wenn Sie mit der Nutzung von Azure CLI 1.0 (azure.js) bereits vertraut sind, wird Ihnen auffallen, dass sich einige Befehle geändert haben.
In einigen Fällen unterscheiden sich die Befehle zum Durchführen einer Aufgabe relativ stark.
Als Hilfe für die Umstellung von Azure CLI 1.0 auf Azure CLI 2.0 haben wir damit begonnen, [diese Befehlszuordnung](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst) zu erstellen.

## <a name="send-us-your-feedback"></a>Senden Sie uns Feedback

```azurecli-interactive
az feedback
```
