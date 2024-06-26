#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 37.  (2023.09.11. - 17.)

---
Damit unsere Termin-App auch den Nutzer benachrichtigen kann, benötigen wir hierfür auch eine Funktion.
Dafür installierten wir das local_notification_plugin Package, dies erspart uns eine eigene Benachrichtigung Logik zu bauen, zusätzlich müssen wir nicht in Kotlin oder Java, eine API programmieren, um auf die Hardware zuzugreifen.  
Für das Nutzten der Lautsprecher und die Benachrichtigung außerhalb der App benötigen Zugriffserlaubnis auf das Smartphone.     
Da Android auf Basis des Linux Kernel läuft, werden die Daten, der Speicherort und die Freigabe einzelner Rechte genauso gehandelt wie bei allen Linux Distributionen.      
In Linux wird die Speicherverwaltung anders geregelt wie unter Microsoft Betriebssystemen. In Linux werden alle Daten direkt auf der Festplatte gespeichert und werden mit Zugriffsrechte belegt.       
Anders als in Windows, wo alle Dateien über das Betriebssystem verwaltet werden, kann unter allen Linux Distributionen, einfach auf der Festplatte Ordner erstellt werden und bearbeitet, damit nicht jeder irgendwelche Schadsoftware auf Linuxsysteme laden kann, um das System zu befallen.      
Um das zu verhindern wird bei Linux basierten Systeme Zugriffsrechte vergeben und damit verhindert das andere Dateien unbefugten zugreifen können.      
Die Zugriffsrechte werden in einer Flutter Anwendung einer Datei namens AndroidManifest.xml verwaltet.      
XML Dateien sind ähnlich aufgebaut wie HTML Dateien, alle Objekte in einen Tag(<…>) geschrieben und haben so lange die Zugehörigkeit zu diesem Element bis dieses beendet wird(…>).     
XML Dateien sind aufgebaut wie HTML Dateien also Parent und Child Objekte werden ineinander verschachtelt und benannt.      
Um nun meiner App die Berechtigung zu geben, dass sie auch außerhalb der App Zugriffsrechte hat auf z. B. die Lautsprecher oder auf die Benachritigungs-Zentrale musste ich in diesem Android Manifest schreiben.       
Ähnlich, aber einfacher funktioniert dies auf dem iOS Betriebssystem, dort muss, allerdings nur angefragt werden.  
Als Nächstes musste ich die Benachrichtigungs-Klasse schreiben, die als API zu dem Package dient, dort definiere ich wie eine Benachrichtigung aussehen soll.       
Um bei den Benachrichtigungen die Töne einstellen zu können, bin ich leider etwas eingeschränkt.        
Deswegen habe ich aus dem Internet lizenzfreie mp.3 Dateien heruntergeladen und in einen neuen Ordner im Android Reiter gespeichert, ähnlich wie ich Assets für eine Windowsapplikation hinterlege.     
&nbsp;
\
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
