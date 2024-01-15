# 21 Windows Client in Azure AD (2 Punkte)

Damit Sie mit dieser Aufgabe starten können, müssen Sie Ihren Client aus der OnPremisis Umgebung erhausnehmen.



Das hinzufügen eines lokalen Clients in Azure AD basiert auf zwei Schritten. Zuerst fügen Sie den Client in die Azure AD mittels Windows Boardmittel. Obwohl sich anschliessend User aus Azure AD am Windows Client anmelden können, kann der Client noch nicht mit Intune verwaltet werden. Dazu benötigen Sie eine Software namens «Company Portal».





# Azure AD-Join (0.5 Punkte)

Nachdem AD-Join können sich Benutzer von der Azure AD anmelden.


![Picture01](/images/21-Picture1.png)


![Picture01](/images/21-Picture2.png)

### Ansicht Geräte im Azure Portal 
https://portal.azure.com/#view/Microsoft_AAD_Devices/DevicesListBlade/mezzoEnabled~/true

![Picture01](/images/21-Picture3.png)


![Picture01](/images/21-Picture4.png)

# Intune Join (1.5 Punkte)

## Company Portal installieren



- Via PowerShell: 
`winget install "company portal" --source msstore --accept-package-agreements --accept-source-agreements`


- Via Windows Store
    - Suchen Sie nach «Company Portal» 

### Starten Sie die Applikation “Company Portal»
### Gerät zu Intune hinzufügen

![Picture01](/images/21-Picture5.png)


![Picture01](/images/21-Picture6.png)

### Überprüfen Sie, ob das Gerät bei Intune angezeigt wird

![Picture01](/images/21-Picture7.png)

### Führen Sie «dsregcmd /status» aus



