# Aufgabe 5: Active Directory erste Schritte (2 Punkt) 

Für diese Aufgabe müssen Sie wissen, wie man Freigaben und Berechtigungen unter Windows verwendet. Falls Ihnen der Unterschied zwischen Freigabe- und NTFS-Berechtigungen nicht bekannt ist, Fragen Sie Ihre Klassenkameraden oder lesen Sie es im Internet nach. Falls Sie nicht sicher sind, Fragen Sie die Lehrperson.





## User und Gruppen anlegen (0.5 Punkt)



- Erstellen Sie Ihre Testbenutzer wie im Portfolio definiert
Falls Sie Probleme mit dem Anlegen der Benutzer haben, weil Ihre Passwörter zu schwach sind, ziehen Sie Aufgabe «9.1 Default Domain Policy - Verändern der Passwortrichtlinien» vor. Falls Sie überfragt sind, kann Ihnen die Lehrperson kurz helfen, da dieses Thema erst später im Modul behandelt wird.

- Erstellen Sie für jede Abteilung, sowie für intern und extern “globale” Sicherheitsgruppen. Intern und extern werden wie die Abteilungen als normale Sicherheitsgruppenerstellt. Anschliessend fügen Sie alle internen Abteilungen in die Gruppe intern und alle externen Abteilungen in die Gruppe extern.

    -  GL (intern) 

    - Aussendienst (extern) 

    - Sekretariat (intern) 

    - Buchhaltung (intern) 

    - Promoter (extern) 

    - Partner (extern) 

    - Informatik (intern) 

    - Messemitarbeiter (extern)

- Fügen Sie die Benutzer in die entsprechenden Gruppen (Siehe Portfolio)

- Fügen Sie die Abteilungsgruppen in Gruppen intern und extern

- Testen Sie einige Benutzer, indem Sie sich mit diesem am Windows 10/11 Client anmelden


## UNC

Sie müssen wissen, wie UNC-Pfade aufgebaut sind und verwendet werden können

- https://de.wikipedia.org/wiki/Uniform_Naming_Convention

- https://gitlab.com/ch-tbz-it/Stud/m159/-/blob/main/02_Unterrichtsressourcen/04_%C3%9Cbungen/%C3%9Cbung UNC.docx



### 

## Ordner und Freigaben erstellen (1 Punkt)

- Erstellen Sie die Ordner- und Freigabestruktur wie in der Tabelle aufgeführt

- Setzen Sie für jede Freigabe die Freigabeberechtigungen für «Jeder» auf «ändern/change»

- Deaktivieren Sie die Vererbung auf der Freigabe «Daten» und allen Unterordnern

- Entfernen Sie die Standardgruppe «Domänenbenutzer»

- Vergeben Sie die NTFS-Berechtigungen aus der Matrix für sämtliche Ordner.

- Es reicht für die volle Punktzahl, nur die Berechtigungen der grün markierten Zeilen zu erfassen


![Table](/images/05-Table1.png)





LB = Laufwerksbuchstabe (Wird erst bei Aufgabe 9 für die Netzlaufwerk benötigt)

R = Read

C = Change

"-"  = Kein Zugriff

## Einige Berechtigungen testen

- Melden Sie sich mit dem Benutzer der Abteilung «Sekretariat» an. Prüfen Sie, ob Sie auf den UNC-Pfad «Buchhaltung» Leserechte haben.

- Melden Sie sich mit dem Benutzer der Abteilung «GL» an. Prüfen Sie, ob Sie auf den UNC-Pfad «Pool» Schreibrechte haben.

- Melden Sie sich mit dem Benutzer der Abteilung «Promoter» an. Prüfen Sie, ob Sie auf das Laufwerk «Aussendienst» keine Rechte haben.

- Machen zwei bis fünf Tests Ihrer Wahl, damit Sie sicher sind, dass alles stimmt.



## ABE (0.25 Punkte)

- Informieren Sie sich über ABE

- Aktivieren Sie anschliessend ABE für alle Freigaben


## Papierkorb (0.25 Punkte)

### Aktivieren Sie den AD-Papierkorb

- Können Sie den Papierkorb wieder deaktivieren? 

- Erstellen Sie einen beliebigen Benutzer und löschen Sie diesen, damit Sie ihn im Papierkorb sehen können



# 

# Kontrolle

Im Video sollen die Aufgaben 5.4, 5.5 und 5.6 gezeigt und erklärt werden.

   ![Kontrolle](/images/Kontrolle.png)





