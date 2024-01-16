
||
| :- |
||

![Bildergebnis für tbz Logo technische berufsschule](Aspose.Words.7eaad7ea-eafa-4211-bef3-05fdb686cffa.001.png)Technische Berufsschule Zürich TBZ

Informationstechnik



![](Aspose.Words.7eaad7ea-eafa-4211-bef3-05fdb686cffa.002.png)IT M159 – 15 ADDS – DNS, Replikation und GPO Fehleranalyse
# <a name="_toc441481075"></a><a name="_toc441483957"></a><a name="_toc441491513"></a><a name="_toc441491633"></a><a name="_toc441494708"></a>15 ADDS - DNS und Replikation Fehleranalyse (2 Punkte)
**15.1 Replmon (0.3 P.)**

15\.1.1 Installieren Sie Replmon «adreplstatusInstaller.msi» auf einem Ihrer Domain Controller

15\.1.2 Führen Sie eine Replication-Statusabfrage durch

15\.1.3 Exportieren Sie das Ergebnis in eine CSV-Datei (Excel)

15\.1.4 Öffnen Sie die CSV-Datei im Excel und speichern Sie einen Printscreen davon im Portfolio.

**15.2 RepAdmin (0.3 P.)**

15\.2.1 Öffnen Sie die CMD als Administrator

15\.2.2 Führen Sie den Befehl «repadmin /replsummary» aus

15\.2.3 Speichern Sie einen Printscreen vom Ergebnis ins Portfolio

**15.3 DCDiag (0.3 P.)**

15\.3.1 Öffnen Sie die CMD als Administrator

15\.3.2 Erstellen Sie einen Ordner tmp auf dem C:\

15\.3.3 Führen Sie den Befehl «dcdiag > c:\tmp\dcdiag.txt» aus

15\.3.4 Öffnen Sie das File «dcdiag.txt» und schauen Sie sich die Ergebnisse genauer an

15\.3.5 Erstellen Sie eine Liste von sämtlichen bestandenen sowie nicht bestandenen Tests und kopieren Sie diese ins Portfolio unter Aufgaben ab.

## **15.4 Gruppenrichtlinien-Eventlog (0.5 P.)**
*Lesen Sie im PDF Gruppenrichtlinien-Kapitel15.pdf das Kapitel 15.5 Gruppenrichtlinien-Eventlog*

15\.4.1 Suchen Sie auf einem Ihrer Clients den Start-Event der Gruppenrichtlinienverarbeitung

15\.4.2 Machen Sie einen Printscreen von der «Correlation-ID» und speichern Sie diesen ins Portfolio

15\.4.3 Suchen Sie auf einem Ihrer Clients den Ende-Event der Gruppenrichtlinienverarbeitung

15\.4.4 Machen Sie einen Printscreen von der «Correlation-ID» und speichern Sie diesen ins Portfolio

**15.5 Active Directory Log Level (0.5 P.)**

*Lesen Sie im PDF Unentbehrliche\_Helfer\_für\_Admins.pdf das Kapitel 7 Der Event Log und die Registry*

15\.5.1 Leeren Sie den Container im Eventviewer unter Anwendungs- Dienstprotokolle -> Directory Service

15\.5.2 Starten Sie einen Ihrer Domaincontrollers neu und zählen Sie sämtliche Ereigniseinträge

15\.5.3 Erhöhen Sie in der Registry wie in Kapitel 7 beschrieben den Event Log Level vom Typ «5 Replication Events» auf Stufe 5.

15\.5.4 Leeren Sie den Container im Eventviewer erneut, unter Anwendungs- Dienstprotokolle -> Directory Service

15\.5.5 Starten Sie einen Ihrer Domaincontrollers nochmals neu und zählen Sie erneut sämtliche Ereigniseinträge unter Anwendungs- Dienstprotokolle -> Directory Service

15\.5.6 Schreiben Sie ins Portfolio, wie hoch die Differenz der Einträge in der Ereignisanzeige zum vorhergegangenen Bootvorgang ist
# Kontrolle:
Erklären Sie Ihre Ergebnisse und Interpretationen im Screencast zu sämtlichen Teilaufgaben.

![Ein Bild, das Rechteck, Reihe, Design, Rahmen enthält.

Automatisch generierte Beschreibung](Aspose.Words.7eaad7ea-eafa-4211-bef3-05fdb686cffa.003.png)
