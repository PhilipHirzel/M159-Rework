## Aufgabe 7a – DC3 zur Gesamtstruktur hinzufügen (1 Punkte)

## Fügen Sie nun den DC(Core) zur Hauptdomäne hinzu. Suchen Sie im Internet selbst nach einer Anleitung. Alternativ können Sie auch folgenden Link verwenden)

<https://docs.microsoft.com/en-us/answers/questions/59818/how-to-install-secondary-domain-controller-as-serv.html>

Install-WindowsFeature -Name AD-Domain-Services -IncludeManagementTools



Install-ADDSDomainController -InstallDns -Credential (Get-Credential DomänenName\administrator) - DomainName DomänenName -SafeModeAdministratorPassword (ConvertTo-SecureString -AsPlainText "Passwort" -Force)


## Kontrolle
   Zeigen Sie folgendes Fenster mit dem neuen Domänencontroller im Video

![IMAGE]()


