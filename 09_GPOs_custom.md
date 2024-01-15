# Aufgabe 9 Mit GPOs arbeiten (4 Punkte) (Praktische Überprüfung)

Falls Sie noch nie mit Gruppenrichtlinien gearbeitet haben, können Sie sich, über die Grundlagen von Gruppenrichtlinien mit den folgendes PDFs informieren.



- Gruppenrichtlinien-Kapitel1.pdf

- Gruppenrichtlinien-Kapitel2.pdf

- Gruppenrichtlinien-Kapitel3.pdf



## 9.1 Default Domain Policy - Verändern der Passwortrichtlinien (1 Punkt)



Grundsätzlich gilt: 

Vermeiden Sie Änderungen an den zwei vorkonfigurierten Gruppenrichtlinien „Default Domain Policy“ und „Default Domain Controllers Policy“, die über das Anpassen der Kennwortrichtlinien hinausgehen. Änderungen in den Default Policies erschweren die Fehlersuche und Behebung. 



Ändern Sie also nur Passwortrichtlinien in der Default Domain Policy. Schalten Sie sämtliche Richtlinien, welche eine Passwortkomplexität verlangen aus. Deaktivieren Sie ebenfalls das Erzwingen von neuen Passwörter nach einer gewissen Zeit. Natürlich sollten Sie dies in der Praxis nicht machen aber für unsere Testumgebung macht es Sinn.



## 9.2 Neue Gruppenrichtlinienobjekte für Netzlaufwerke (1 Punkte)

Für diese Aufgabe lesen Sie bitte vorher den Abschnitt «5.4 Benennung von GPOs» in Gruppenrichtlinien-Kapitel5.pdf. 

Wenn Sie neue Gruppenrichtlinienobjekt erstellen, beachten Sie die Punkte aus dem Kapitel 5.4 für eine sinnvolle Benennung.



Folgende Netzlaufwerke sollen für die Mitarbeiter zur Verfügung stehen



- «Pool» unter dem entsprechenden Laufwerksbuchstaben für die ganze Firma

- Jede Abteilung soll Ihr Abteilungslaufwerk haben

- Alle Interne Abteilungen sollen das Laufwerk Intern haben

- Alle Externe Abteilungen sollen das Laufwerk Extern haben

- 

## 9.3 Verknüpfung «CRM» auf dem Desktop verteilen mittels positiver Sicherheitsfilterung (1 Punkt)



Falls Sie nicht wissen, wie die positive Sicherheitsfilterung funktioniert, lesen Sie die Erklärung zur «Positiven Sicherheitsfilterung» unter «Kapitel 3.4.5.1 Positive Sicherheitsfilterung» und 5.2.2 GPOs und Sicherheitsfilterung.



Ihre Firma arbeitet mit einem Web-CRM(«https://crm.webapp.ch»). Erstellen Sie nun ein GPO für das Erstellen dieser Verknüpfung auf dem Desktop und verknüpfen Sie die GPO auf oberster Ebene. Mit der positiven Sicherheitsfilterung sollen nun Gruppen zur Filterung hinzugefügt werden, damit diese Abteilungen die Verknüpfung automatisch erhalten. 

Entfernen sämtliche Gruppen und Testen Sie das Ganze mit der Gruppe «intern».







9.4 GPO mit WMI-Filter erstellen und anwenden (1 Punkt)



Lesen Sie für diese Aufgabe Kapitel «4.3 WMI-Filter» durch.



- Legen Sie einen WMI-Filter an, welcher überprüft, ob es sich um eine Windows10 Installation handelt.  (Infos im Buch, Seite 50 im Kapitel «4.3 WMI-Filter»:



- Erstellen Sie anschiessend ein neues GPO-Objekt mit dem Namen “Textdatei kopieren” und verknüpfen Sie dieses mit der OU-Promoter. Auf dieses neue GPO-Objekt soll der WMI-Filter angewendet werden. 



- Erstellen Sie anschliessend auf der Freigabe Pool eine neue Textdatei mit dem Namen “WMI-Filter.txt”.  Der Inhalt der Datei kann leer sein.



- Das GPO-Objekt “Textdatei kopieren”, soll nun bei sämtlichem User der OU Promoter, die Textdatei “WMI-Filter.txt” in das Verzeichnis mit der Variable %temp% kopieren. 



#### Damit die GPO von 9.4 funktioniert, müssen zwei Dingen berücksichtigt werden

- Der Der Dateiname “WIM-Filter.txt” muss auch beim Zielpfad angegeben werden

- Im Sicherheitskontext des angemeldeten Benutzers ausführen muss unter “Geminsame Optionen” aktiviert sein, damit man mit der Variable %temp% arbeiten kann



# Kontrolle 9.1-9.3

 IMAGE



# Kontrolle 9.4



- Exportieren Sie zusätzlich zum Screencast eine HTML-Datei mit dem Befehl auf einem Ihrer Clients 

- gpresult /h «gpo.html»



- Speichern Sie die HTML Datei in Ihrem privaten Kanal im Teams.



