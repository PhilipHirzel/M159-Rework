# 13 Farbige und SW Drucker per GPO verteilen (1 Punkt)



# 13.1 Ausgangslage

Sie möchten auf dem Server zwei freigegebene Drucker via GPO an die Benutzer verteilen. Dabei möchten einmal einen Drucker verteilen, welcher per Standardeinstellung «schwarz» druckt und ein anderer Drucker, welcher automatisch «farbig» druckt. Der Endbenutzer, soll zwei verschiedene Drucker zur Verfügung haben, welche schlussendlich, auf dasselbe (fiktive) Endgerät, mit unterschiedlicher Farbeinstellung drucken.

Hinweis: Falls Ihnen nicht bekannt ist, wie man auf dem Server einen TCP/IP-Drucker installiert (Es kann eine fiktive IP-Adresse verwendet werden), gibt es im GIT Repo unter  eine Anleitung (Netzwerkdrucker_einrichten.docx

#  Auftrag

### 13.2.1 Drucker auf dem Server einrichten

Installieren einen beliebigen „fiktiven“ Farblaserdrucker zwei Mal unter einer fiktiven IP-Adresse. 

Nun können Sie pro Drucker in den Einstellungen die Farbeinstellungen definieren und den Drucker so benennen. Achtung: Damit die Einstellungen auch beim User ankommen müssen Sie die Werte unter Standardwerte anpassen. Siehe Printscreen

![Picture01](/images/13-Picture1.png)

Wenn Sie nicht wissen, wie man einen TCP/IP Drucker installiert finden Sie eine Anleitung in MS Teams unter Tools.



Geben Sie die Drucker unter diesem Namen frei.

- Drucker_Farbe

- Drucker_SW







## GPO für die Verteilung der Drucker einrichten



Wenn Sie Ihre Drucker konfiguriert haben, können Sie die Verteilung mittels GPO in Angriff nehmen.

- Einstellungen => Systemsteuerungseinstellungen => Drucker 

Klicke dort mit der rechten Maustaste auf Drucker und anschließend auf 

„Neu“ + „Freigegebener Drucker„.

![Picture01](/images/13-Picture2.png)

Es öffnet sich das Fenster „Neue Eigenschaften für freigegebene Drucker“ in welchem Du nun den Drucker als UNC-Pfad angeben kannst mit \\FQDN\Druckerfreigabename

Unter Aktion kannst Du entweder Aktualisieren oder Ersetzen auswählen. Den korrekten Freigabepfad erhältst Du, indem Du auf die drei Punkte […] klickst und den gewünschten Drucker aus dem Verzeichnis wählst. Die Option „Drucker als Standarddrucker festlegen“ wähle ich in diesem Schritt noch nicht aus.



![Picture01](/images/13-Picture3.png)


# Kontrolle

Wenn Sie die Drucker auf dem Client unter dem entsprechenden AD-Benutzer sehen, hat die Verteilung via Gruppenrichtlinie funktioniert. 
Löschen Sie nun die Drucker manuell und führen Sie ein «gpupdate /force» durch, um festzustellen, dass die Drucker erneut angelegt werden. Machen Sie ein Video von diesem Prozess und speichern Sie den Pfad in Portfolio.

**Tipp:**
Dies funktioniert nur wenn Sie beim GPO Objekt «replace» oder «update» verwendet haben.



