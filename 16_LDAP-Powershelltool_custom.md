# Übung 16

# 16.1 LDAP-Abfragen / LDAP-Queries (CMD-Prompt) (1 Punkt)

![Picture01](/images/16-Picture1.png)

Damit Sie diese LDAP-Befehle in der CMD ausführen können, müssen Sie die RSAT Tools für Ihren Server installieren. Sie finden eine Anleitung dazu im Ordner Tools.







## Auftrag 16.1.1: 

Erstellen Sie folgende vier AD-Objekte mit Dsadd:



- User

- Computer

- Kontakt

- Gruppe





## Auftrag 16.1.2:

Schreiben Sie eine LDAP-Abfrage mit «Dsquery», welche sämtliche User einer von Ihnen erstellten OU ausgibt



Schreiben Sie eine LDAP-Abfrage mit «Dsquery», welche sämtliche Computer einer erstellten OU ausgibt



## Auftrag 16.1.3:

Fügen Sie mit Dsmod einen User in eine Gruppe.



Auftrag 16.1.4:

Geben Sie einige Eigenschaften Ihrer Wahl des Kontaktes, welcher in Auftrag 1 erstellt wurde, mit DSget aus

## 

Auftrag 16.1.5:

Führen Sie die Beispiele (Examples) aus, welche unter dem QR-Code von «Dsmove» zu finden sind. Adaptieren Sie die Beispiele auf Ihre eigenen Objekte. 

Rename a user object from XY to YZ

Move the user object for XY from XY to the YZ organization

To combine the rename and move operations



Auftrag 16.1.6:

Löschen Sie mit «Dsrm» ein Testobjekt Ihrer Wahl



# Kontrolle

Dokumentieren Sie sämtliche Schritte also «Input und Rückmeldung» der LDAP-Abfrage mit Printscreens in einem separaten Dokument. Speichern Sie dieses Dokument mit der Namenskonvention «vorname.nachname» in Ihrem privaten Teams Kanal ab.

Erstellen Sie zusätzlich ein Screencast Video mit zwei Beispiel, um zu zeigen, dass Sie in der Lage sind, diese Befehle selbstständig auf Ihrer Umgebung auszuführen.






# 16.2 LDAP-Abfragen / LDAP-Queries (PowerShell) (4 Punkte)

Importieren Sie das Modul für Active Directory unter PowerShell.





![Picture01](/images/13-Picture2.png)





## Auftrag 16.2.1

Erstellen Sie ein PowerShell-Tool, welches diverse AD-Aufgaben ausführen kann. Das PowerShell Tool soll ein Menu haben, dass entweder mit der Maus(grafisch) oder mit der Tastatur (Konsole) bedient werden kann.



Erstellen Sie eine Bedienungsanleitung im Portfolio unter Punkt 7.



Folgende Menüpunkte soll das Tool besitzen:



- 1. Neuen User erstellen

- 2. Bestimmten User löschen

- 3. Alle User von einer OU anzeigen

- 4. Alle User von einer Sicherheitsgruppe anzeigen

- 5. User von einer Excel-Tabelle in das Active Directory importieren (Optional)



#### Beschreibung der einzelnen Menüpunkte


- Neuen User erstellen: 
Nachdem diese Optionen gewählt wurde, soll der Benutzer nach den Eigenschaften für das neue Userobjekt schrittweise oder auf einmal abgefragt werden. Welche Eigenschaften Sie für das Userobjekt festlegen, ist Ihnen überlassen. Zwingend vorhanden muss aber sein:



- OU (In welcher der User angelegt wird)

- Login

- Passwort

- Vorname

- Nachname

- Telefonnummer


- Bestimmten User löschen:
Nachdem diese Option gewählt wurde, soll der Benutzer nach dem Benutzername (sAMAccountName) des zu löschenden Users gefragt werden und nach dem erfolgreichen löschen soll eine Bestätigung erfolgen.



- Alle User von einer OU anzeigen
Nachdem diese Option gewählt wurde, soll der Benutzer nach der OU gefragt werden. Wenn Sie erfahren sind können Sie eine Liste mit sämtlichen OU anzeigen und der User kann eine davon auswählen. Wenn Sie das Tool einfach halten möchten dann Fragen Sie den User mit einer Input-Box nach der OU die ausgelesen werden soll.


- Alle User von einer Sicherheitsgruppe anzeigen
Identisch wie Menüpunkt 3 einfach für Sicherheitsgruppen.


- User von einer Excel-Tabelle in das Active Directory importieren (Optional)
Nachdem diese Option gewählt wurde soll entweder einen Pfad abfragt oder mit einem Fenster eine Datei ausgewählt werden können. Eine Liste von Benutzer, welche in dieser CSV Datei enthalten sind, sollen in eine bestimmte OU importiert werden. 



# Kontrolle

- Machen Sie ein Screencast wie man das Tool im Einsatz sieht und wie Sie die erforderlichen Funktionen ausführen.

- Speichern Sie das PowerShell Tool in Ihrem privaten Teams Kanal ab.

