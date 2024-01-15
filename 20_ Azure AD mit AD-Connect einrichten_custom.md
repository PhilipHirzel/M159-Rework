# 20_Azure AD & AD Connect (2 P.)

Bei dieser Aufgabe verbinden Sie Ihre on premises AD-Umgebung mit dem Azure AD inkl. Office365 Integration. Ziel ist es, dass Ihre lokalen Benutzer in die Cloud synchronisiert werden und automatisch eine Office Lizenz gewissen Benutzern zugewiesen wird.



## Account erstellen (1 Punkt)

Gehen Sie auf die Seite  und registrieren sie eine neue Developer Umgebung. Erstellen Sie im Portfolio einen neuen Abschnitt für diese Daten/Logins. 

Achtung: Die Registration führt im TBZ-Netzwerk zu einem Fehler bei der Überprüfung Ihrer Mobile-Nummer (Security check fail), registrieren Sie sich mit einem Hotspot, dann sollte es gehen.

|  |  |
| ----------- | ----------- |
| **IMAGE** | Melden Sie sich mit einem bestehenden Microsoft Account an oder erstellen Sie einen neuen Account. Falls Sie einen neuen Account erstellen, verwenden Sie als Domain «outlook.com»|
| ![Picture01](/images/20-Picture1.png) | Falls Sie einen neuen Account erstellen, füllen Sie die Daten entsprechen aus.|
| ![Picture01](/images/20-Picture2.png) |          |
| ![Picture01](/images/20-Picture3.png) | Wählen Sie «Instant Sandbox»|
| ![Picture01](/images/20-Picture4.png) | Setzen Sie ein Passwort für Ihren Azure Admin. Notieren Sie sich diese Angaben im Portfolio unter dem neuen Abschnitt. |
| ![Picture01](/images/20-Picture5.png) | Richten Sie Zwei-Faktor-Authentifizierung ein |
| ![Picture01](/images/20-Picture6.png) | Wenn die Einrichtung erfolgreich abgeschlossen wurde, sollten Sie folgendes Bild sehen. Sie sehen hier wie lange Ihre Sandbox bzw. Ihre Testumgebung läuft|
| ![Picture01](/images/20-Picture7.png) |  	Melden Sie sich nun mit Ihrem Azure-Administrator bei Azure an, um einen ersten Einblick zu erhalten. https://azure.microsoft.com/de-de/services/active-directory/ oder https://entra.microsoft.com/  Beim ersten Login müssen Sie noch die Microsoft Authenticator App einrichten. Installieren Sie die App auf Ihrem Smartphone und scannen Sie den QR-Code. Nachdem erfolgreichen einrichten, sehen Sie Ihr Admin-Konto in der Authenticator App|
| ![Picture01](/images/20-Picture8.png) |Wenn Sie nun Azure AD öffnen, sehen Sie die 20 vordefinierten Testbenutzer. Wir werden diese Benutzer aber nicht benötigen, sondern wollen nun eine Synchronisation aus unserer AD-Umgebung ins Azure einrichten.
## AD Connect auf einem Domänencontroller installieren (1 Punkt)
|  |  |
| ----------- | ----------- |
| https://www.microsoft.com/en-us/download/details.aspx?id=47594 AD Connect V2 wurde im Oktober 2023 durch Microsoft veröffentlich. Das Setup hat etwas geändert. Lassen Sie sich dadurch aber nicht beirren. Die Schritt für Schritt Anleitung an dieser Stelle hier wird bei Gelegenheit aktualisiert. |   Laden Sie die Datei AzureADConnect.msi herunter       |
|  | Installieren Sie das Paket AzureADConnect.msi |
| **IMAGE** | Wählen Sie Anpassen|
| ![Picture01](/images/20-Picture9.png) | Melden Sie sich nun mit dem Azure-AD Administrator an.       |
| ![Picture01](/images/20-Picture10.png) | Evtl. öffnet sich ein Popup für die Authentifizierung mittels Authenticator App.      |
| ![Picture01](/images/20-Picture11.png) |  Wählen Sie Kennwort-Hashsynchronisierung|
| ![Picture01](/images/20-Picture12.png) |  Sie sollten nun in der Lage sein, Ihre Gesamtstruktur für die Synchronisation auszuwählen        |
| ![Picture01](/images/20-Picture13.png) |  Erstellen Sie einen Benutzer für die Synchronisation z.B. “AdSyncAdmin” Geben Sie einen Benutzer an, der die Rolle Unternehmensadministrator» und “besitzt.|
| https://learn.microsoft.com/en-us/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization?view=o365-worldwide | Fügen Sie einen weiteren UPN-Suffix hinzu         |
| ![Picture01](/images/20-Picture14.png) | Starten Sie den Synchronisation Service und machen Sie einen Printscreen der letzten Synchronisation         |
| **IMAGE** | Überprüfen Sie nach der erfolgreichen Synchronisation mit Azure AD, ob Sie Ihre lokalen User und Gruppen in Azure AD finden können. https://entra.microsoft.com/ Melden Sie sich mit dem Aussendienstbenutzer bei https://www.office.com/ an.|






















