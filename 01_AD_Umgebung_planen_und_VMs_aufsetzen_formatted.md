# Aufgabe 1 – Planen und VMs vorbereiten

## Einleitung:

In diesem Modul bauen Sie Ihre Active Directory Umgebung schrittweise auf. Das Modul 159 ist modular aufgebaut, dass bedeutet, Sie können selbst bestimmen, welche Aufgaben und somit auch welche Konfiguration Sie installieren. 

Das Ganze beginnt mit einer sorgfältigen Planung. In der Portfolio-Vorlage finden Sie leere Felder, welche Sie ausfüllen müssen, damit Ihre Planung abgeschlossen werden kann. 



Anbei erhalten Sie einen Überblick über Ihre zukünftige Umgebung. 



- Eins bis zwei Standorte

- Ein bis vier Domänenkontroller (2 DCs an Standort 1 und 2 DCs an Standort 2)

- Einen «Domain Tree» bestehend aus zwei Domänen (1x Hauptdomäne und 1x Subdomäne)

- Pro Standort ein Windows 10 Client (Nicht im Bild enthalten)

![Picture1](/images/01-Picture1.png)

In der Grafik oben sehen Sie Ihre lokale Installation ohne Azure, wenn Sie zwei Standort und die Subdomain einrichten.

Diese Namen in der Grafik sind nur **Beispiele** und sollen von Ihnen neu und individuell gestaltet werden.


## Aufgabe Spezifikationen (1 Punkt) (Portfolio)

Füllen Sie im Portfolio, Punkt 3 Spezifikationen der Systeme aus.

Lesen Sie , auf was Sie bei der Wahl Ihres Domänenamen achten, sollten

Im Modul 159 möchten wir zwei Standorte simulieren. Sie können die Standorte frei wählen, zum Beispiel Zürich und Genf. Jeder Standort hat sein eigenes Subnetz, welches mit einem Router verbunden ist. Ein logisches Beispiel-Netzwerklayout finden Sie unter Punkt 2.2 in den Aufgaben im Repository.



**Hinweis**: Füllen Sie das Portfolio komplett aus, auch wenn Sie später nicht alle Domänen, Maschinen und Standorte nicht installieren bzw. konfigurieren.



## Logische AD/Netzwerklayout (1 Punkt) (Portfolio)

Erstellen Sie mit Microsoft Visio oder mit [draw.io](draw.io) ein kombiniertes AD- und Netzwerklayout Ihrer kompletten Umgebung. Achten Sie darauf, dass sämtliche Standorte, Domänennamen, Computernamen (FQDN), IP-Adressen, Netzadressen und virtuelle Netzwerke im Layout vorhanden sind. 





## Aufsetzen der VMs (1 Punkt) (Praktische Überprüfung)

Setzen Sie die rohen VMs auf.

Iso Files können mit dem TBZ-Login unter: https://azureforeducation.microsoft.com/devtools
heruntergeladen werden



## Standardeinstellungen (1 Punkt) (Praktische Überprüfung)

Folgende Einstellungen müssen Sie auf sämtliches System vornehmen. Auf dem «Windows Core Server» müssen Sie lediglich 1.4.1 und 1.4.2 einstellen.



### Server (Core / Desktop)

#### Firewall (Core & Desktop)

- Ping erlauben

### Tastaturlayout (Core & Desktop)

- CH

### Verstärkte Sicherheitskonfiguration für IE (Desktop)

- Im Server Manager Ausschalten

### Netzwerkadapter (Core & Desktop)

- Deaktivieren Sie TCP/IP V6

### Anzeige & Ordneroptionen (Desktop)

- Deaktivieren «Erweiterungen bei unbekannten Dateitypen ausblenden»

- Deaktivieren «Freigabeassistenten verwenden»

- Deaktivieren «Geschützte Systemdateien ausblenden»

- Erstellen Sie eine Verknüpfung für CMD auf dem Desktop

- Blenden Sie alle Desktopsymbole ein


### Client

###  Firewall

- Ping erlauben



### Tastaturlayout

- CH

### Netzwerkadapter

- Deaktivieren Sie TCP/IP V6

### Ordneroptionen

- Deaktivieren «Erweiterungen bei unbekannten Dateitypen ausblenden»

- Deaktivieren «Freigabeassistenten verwenden»

- Deaktivieren «Geschützte Systemdateien ausblenden» Erstellen Sie eine Verknüpfung für CMD auf dem Desktop

- Erstellen Sie eine Verknüpfung für CMD auf dem Desktop

- Blenden Sie alle Desktopsymbole ein

### Deaktivieren Sie “UAC” (Unterste Stufe)



## Spezifizierte Konfiguration auf den VMs festlegen (1 Punkt) (Praktische Überprüfung)

Machen Sie die Einstellungen auf den VMs, welche Sie im Portfolio unter Punkt 1 festgelegt haben.

Bereiten Sie Ihre Server für das Aufsetzen einer AD-Gesamtstruktur vor. Im Video «Active Directory-Installation vorbereiten.wmv» wird Ihnen gezeigt, was dazu alles gemacht werden muss. 
**Hinweis: Ihre DNS-Zone für das AD muss nicht wie im Video gezeigt vorher manuell erstellt werden**

**Pro Tipp: Erstellen Sie nach dieser Aufgabe Backup bzw. Checkpoint/Snapshots von Ihren VMs, damit Sie im Falle wieder auf diesen Zustand zurückkehren könnten.**



# Kontrolle:
  

Zusätzlich muss das Portfolio **Abschnitt 1.1** für die Kontrolle dieser Aufgabe ausgefüllt und im MS Teams in Ihrem persönlichen Kanal abgelegt sein.

