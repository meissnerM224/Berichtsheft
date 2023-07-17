#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 30.  (2023.07.24. - 30.)

---
Das Proxy-Pattern wird verwendet, wenn das eigentliche Objekt verschleiert werden soll.     
Z.B. bei einem Passwort abfrage. Die einzelnen Ziffern verschleiern soll, hier wird klassisch ein Stern als Stellvertreter für die Ausgabe aufgerufen, dieser Stellvertreter zeigt nach außen ein Sternsymbol an, aber intern wird eine Ziffer in ein Passwort Formular weiter gereicht.        
Mit dem Proxy-Pattern kann die Flexibilität, die Sicherheit und die Performance verbessert werden.      
Der Stellvertreter kann eingesetzt werden, um Ladezeiten zu überbrücken.        
Z.B. kann bei einem Internet Anfrage etwas Zeit vergehen, damit aber der Nutzer nicht unnötig warten muss, könnte hier schonmal ein Remote Proxy angezeigt werden, um die Funktionalität während des Ladens aufrechtzuerhalten und wenn das eigentliche Objekt erstellt wird.       
Anschließend kann der Proxy mit dem eigentlichen Objekt getauscht werden.       
Dies hat aber auch zur Folge, dass etwas mehr Rechenleistung bzw. ein Overhead entsteht.        
Es wird zusätzlich kompliziert, da die Implementation des Proxys vielleicht die eigentliche Funktion unnötig kompliziert aussehen lässt.        
Ähnlich wie das Proxy Pattern das Programm nach innen undurchsichtig macht, kann auch das Fassade-Pattern benutzt werde.        
Bei dem Fassade-Pattern wird unnötig viele Interaktion mit verschiedenen Stellen im Code verhindert bzw. über eine Fasade abgefangen oder umgeleitet.       
Hierbei wird ein Objekt erstellt, das entwickelt wurde, um die Interaktion mit dem Nutzer zu erleichtern.       
Wie eine Hausfassade, alle Steine, Kabel, Rohre oder sonstiges Innenleben eines Hauses verdeckt, wird hier auch ein Objekt erstellt, meist ein Singelton.       
Dieses Objekt dient dann als API für den Nutzer, der mit dem Programm interagieren kann und auf der anderen Seite das Programm ordnen und strukturieren kann.       
&nbsp;
\
\
\
\
\
\
\
\
\
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
