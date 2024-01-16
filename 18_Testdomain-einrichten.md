# 18 Testdomäne einrichten (5 Punkte)

*Die Testdomäne ist eine “Child-Domain", sprich eine untergeordnete Domäne Ihrer Hauptdomäne.*

*Damit dies ohne Probleme funktioniert, müssen Sie zuerst den DNS-Server von der Hauptdomäne beim DC der Testdomäne korrekt einrichten und die Namensauflösung in beide Richtungen testen. Falls der DC von der Hauptdomäne ohne Probleme aufgelöst werden kann, können Sie mit der Installation beginnen. Der DC auf dem Sie die “Child-Domain” installieren, muss nicht aufgelöst werden können.*

 # Testdomäne einrichten und mit Client beitreten (2 Punkte)
    ## Installieren Ihrer “Child-Domain”
Installieren Sie auf dem DC4 beim Standort 1 eine “Child-Domain” nach der Vorgabe, welche Sie im Portfolio gemacht haben.
 ## Treten Sie nun mit dem Client von Standort 1 der Testdomäne bei


 Adminrechte in Testumgebung für Abteilung “IT” aus Hauptdomäne	
   `	`(2 Punkte)
   ===============================================================
    ## Erstellen Sie eine neue Organisationseinheit “Testcomputer” und fügen Sie den Client 
      ## in diese neue OU. Erstellen Sie ein neues GPO-Objekt mit dem Namen “IT-lokale-Adminrechte"
    ## Und verknüpfen Sie dieses mit der OU “Testcomputer”.

    ## Erstellen Sie auf der GPO “IT-lokale-Adminrechte" die Einstellung, dass alle User aus der
      ## Sicherheitsgruppe “IT” von der Hauptdomäne, Adminrechte auf den lokalen Clients der OU 
## “Testcomputer” haben. Eine englische Anleitung finden Sie am Ende dieser Aufgabe 18.

 ## Erstellen Sie dasselbe in der “Default Domain Controllers Policy”

 ## Sorgen Sie dafür, dass die Abteilung IT auch die “Default Domain Policy” bearbeiten kann.

##
Anleitung Benutzer aus Hauptdomäne zu den Administratoren in der Testdomäne hinzuzufügen:

- Create and link a GPO at the root of the child domain (actually, link it to a sub-OU with a test computer in it first, then when you know it's working, link it to the root of the domain).

- In that GPO, open "Computer Settings", then "Windows Settings", "Security Settings", and "Restricted Groups".

- Right-click "Restricted Groups" and do an "Add Group".

- Click "Browse" in the "Add Group" dialog, key in "Administrators" (**not** "Domain Admins" or anything else), and click "Check Name" and "OK". Click "OK" to dismiss the "Add Group" dialog.

- In the "Administrators Properties" dialog, click the "Add" button at the top, beside the "Members of this Group" list-box.

- Click "Browse" in the "Add Member" dialog and key in "Domain Admins" and click "Check Name" and "OK". In the "Add Member" dialog, you'll see "CHILDDOMAINNETBIOSNAME\Domain Admins" listed. Click "OK".

- In the "Administrators Properties" dialog, click the "Add" button at the top, beside the "Members of this Group" list-box again.

- Click "Browse" in the "Add Member" dialog and key in the name of the global group in the parent domain that you created to hold users who are getting "Administrator" rights in the child domain. Before you click "Check Name", click "Locations" and choose your parent domain in the "Locations" dialog and click "OK". Then click "Check Name" and "OK". In the "Add Member" dialog, you'll see "PARENTDOMAINNETBIOSNAME\Group name you created" listed. Click "OK".

When this GPO applies to computers, their local "Administrators" group will get the groups "CHILDDOMAINNETBIOSNAME\Domain Admins" and "PARENTDOMAINNETBIOSNAME\Group name you created" nested into it automatically.


 Freigabe erstellen und Gruppe aus Hauptdomäne berechtigen 
   `	 `(0.5 Punkte)
   ==========================================================
    ## Erstellen Sie eine Freigabe mit dem Namen “Labor” auf dem DC der Testumgebung. Denken Sie
      daran, die Freigabeberechtigungen auf “Jeder hat Change”, zu setzen
    ## Geben Sie der Gruppe Partner aus der Hauptdomäne schreibrechte auf diese Freigabe

 # Erstellen einer “Universalen Gruppe” (0.5 Punkte)
    ## Erstellen Sie auf der Testumgebung eine “Universale Gruppe” mit dem Namen “Testgruppe”
    ## Erstellen Sie einen User Ihrer Wahl auf der Testumgebung und fügen Sie diesen in die Testgruppe.
    ## Fügen Sie die Abteilung Aussendienst ebenfalls in diese universelle Gruppe
    ## Erstellen Sie eine neue Freigabe mit dem Namen Test-Universal auf der Hauptdomäne und fügen Sie
      ## diese universelle Gruppe mit Leserechten hinzu
