# Aufgabe 3: Neue Gesamtstruktur aufsetzen (DC1) (2 Punkte) 


Unter einer neuen Gesamtstruktur versteht man eine neue Domäne aufsetzen. 
Achtung: Weitere DCs werden erst später in die Domäne aufgenommen.


### Video zur Aufgabe 3

[Einen ersten Domänencontroller installieren](https://gitlab.com/ch-tbz-it/Stud/m159/-/blob/main/02_Unterrichtsressourcen/03_Fachliteratur&Tutorials/Videos.md)



## AD DS-Rolle auf dem DC1 hinzufügen

- Server Manager Rolle hinzufügen



## DC1 promoten (1 Punkt)

- Neue Gesamtstruktur

- Domainname Spezifikationen (a-z, 0-9, ‘-‘)

- Standardspeicherorte belassen



## DNS (0.5 Punkt)

- Richten Sie eine DNS-Weiterleitung an 8.8.8.8 (oder alternative Ihrer Wahl) für Ihren ersten DNS-Server ein.

- Forward-Zone einrichten (Wird beim Promoten eines DC automatisch erstellt)
-
- Für Jedes Subnetz müssen Sie eine «Reverse-Zone» einrichten
-
- Wenn Sie Ihren DC in der Forward-Zone finden, machen Sie eine Aktualisierung des PTR-Records, damit der Host auch in der Reverse-Zone zu finden ist.

- «NS LOOKUP» auf dem Server vorwärts und rückwärts testen



### Ändern Sie den Namen des Administrators auf den von Ihnen vorgesehenen Namen ab (0.5 Punkte)





# Kontrolle:

  ![Kontrolle](/images/Kontrolle.png)

