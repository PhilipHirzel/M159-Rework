# Aufgabe 17 – DFS einrichten und Azure File Sync einrichten (3 Punkte)

Schauen Sie für diese Aufgabe das DFS-Einrichten Video an unter



 



# DFS einrichten, Namespace anlegen und GPO anpassen (1 Punkt)



## Rolle hinzufügen

Fügen Sie Ihrem DC1, die Rolle «DFS-Namespaces»

## Namespace erstellen

Erstellen Sie einen Namespace ihrer Wahl

## Freigabe hinzufügen

Fügen Sie Ihre bestehende Freigabe «Daten», ihrem neuen Namespace hinzu

## GPO-Netzlaufwerk anpassen

Passen Sie die Gruppenrichtlinie mit dem Netzlaufwerkes so an, dass nun neu, der Pfad mit dem neuen Namespace verwendet wird. Überprüfen Sie das Ergebnis auf dem Client mit «GPUPDATE».



# Kontrolle

Zeigen Sie im Video die Einrichtung und den Zugriff über neuen Namespace








# Azure Storage & File Sync einrichten (2 Punkt)

Leider gibt es bei dieser Aufgabe beim Hinzufügen des Servers einen Fehler. Die Punkte erhalten Sie aber trotzdem, wenn Sie es bis dorthin schaffen.


https://www.youtube.com/watch?v=nfWLO7F52-s
Sie sollen nun den DFS-Namespace mit Azure synchronisieren



## Azure File Sync Agent herunterladen
https://aka.ms/afs/agent



## Azure File Sync Agent auf dem Server installieren


![Picture01](/images/17-Picture1.png)


## Erstellen Sie einen Storage Account in Azure (Storage Account / Speicherkonto)

- Verwenden Sie hierfür Ihr TBZ-Account und aktivieren Sie die kostenlose Azure-Umgebung

- Gehen Sie zu Alle Ressourcen und installieren Sie Ihr neues Speicherkonto / Storage Account


![Picture02](/images/17-Picture2.png)

- Gehen Sie zu Alle Ressourcen und installieren Sie Ihr neues Speicherkonto / Storage Account

![Picture02](/images/17-Picture3.png)

- Verwenden Sie nicht wie im Printscreen Daten als Speicherkontoname da dieser Name eindeutig sein muss. Alle restlichen Einstellungen können Sie auf «Standard» belassen.



## Erstellen Sie nun im Storage Account einen File Share / Dateifreigabe

- Gehen Sie auf Ihre Ressource

- Gehen Sie zu File Share / Datei Freigaben

- Erstellen Sie eine neuen File Share / Dateifreigabe 

![Picture03](/images/17-Picture4.png)



## Azure File Sync einrichten

- Gehen Sie wieder auf Alle Ressourcen -> erstellen

- Suchen Sie nach Azure File Sync

![Picture04](/images/17-Picture5.png)

## Server registrieren und Azure Sync einrichten

- Gehen Sie zurück zum Server

- Wählen Sie «Sign in» für AzurCloud

![Picture05](/images/17-Picture6.png)

- Melden Sie sich mit Ihrem Azure Account an und registrieren Sie Ihren Server

![Picture05](/images/17-Picture7.png)

- Anschliessend sehen Sie Ihren Server unter «Registrierte Server»

- Gehen Sie zurück zu Azure auf Sync group / Synchronisierungsgruppen -> Neue hinzufügen

- Füllen Sie die erforderlichen Felder aus

- Fügen Sie einen Serverendunkt hinzu geben Sie dabei 

![Picture05](/images/17-Picture8.png)

# Kontrolle

- Zeigen Sie den registrierten Server in der Azure Cloud. Erstellen Sie anschliessend eine Datei lokal auf dem on-prem Server und zeigen Sie im Video wie diese in die Cloud synchronisiert wird.

