# Aufgabe 2 – «pf sense» installieren und konfigurieren – 1 Punkt
1. ## **ISO-Datei herunterladen**

- <https://www.pfsense.org/download/>


1. ## **Neue virtuelle Maschine erstellen**
- Zwei oder drei Netzwerkadapter (Konfiguration «VMnet» beachten)

  *Zwei Adapter = Wie im Portfolio definiert*

*Drei Adapter = Ihre Umgebung hat zusätzlich noch ein Internetanschluss*

- Boot type BIOS (Nicht UEFI)
- 8GB Harddisk
- 1GB Ram
  1. ## **ISO installieren**


1. ## **«pf sense» Konfiguration**
- Konfigurieren Sie die IP-Adressen die erste LAN Schnittstelle

![iMAGE](https://github.com/PhilipHirzel/M159-Rework/blob/7b9fb6e466d6b6e4bf65ea5239fdb35a28e5f1c7/images/02-Picture01.png)

- Nun können Sie über das Webinterface zugreifen und weitere Interfaces «assignen»

user: admin

pass: pfsense


![iMAGE]([images/02-Picture02.png](https://github.com/PhilipHirzel/M159-Rework/blob/50642edd119fd225c9577982226f3cd74d3e94ef/images/02-Picture02.png))

- Konfigurieren Sie «Regeln»

![iMAGE](images/[02-Picture03.png](https://github.com/PhilipHirzel/M159-Rework/blob/50642edd119fd225c9577982226f3cd74d3e94ef/images/02-Picture03.png))

![iMAGE](images/[02-Picture04.png](https://github.com/PhilipHirzel/M159-Rework/blob/50642edd119fd225c9577982226f3cd74d3e94ef/images/02-Picture04.png))


1. ## **Firewall Regel kopieren**
   Für das erste Interface erstellt «pfsense» automatisch eine «Default allow to any» Regel. Kopieren Sie diese Regel fürs zweite Interface und passen Sie die Schnittstelle und das Netzwerk an.


1. ## **Routing testen**
Pingen Sie Server 1 von Server 2 aus und umgekehrt. Falls der ping ankommt, ist das Routing korrekt eingerichtet. 

***Achtung:** Machen Sie ein Backup, Snapshot oder Checkpoint vom Router, wenn er funktioniert.*


# **Kontrolle:**
Beim Video muss ersichtlich sein, dass es sich um Ihre Umgebung handelt.

` `![IMAGE](images/Kontrolle.png) 

