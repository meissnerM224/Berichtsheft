#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 13.  (2023.03.27. - 04.02.)

---
Meine Aktuelle Aufgabe( bugfix bei einer Passwort zurücksetzten event ), welche ich in unserem aktuellen
Projekt gewählt habe, weil mich interessierte wie eine Link in einer Email auf ein Programm zugreifen kann.
Bei dem Versuch die Logik hinter der Funktion zu verstehen die, diese Email versendet bin ich jedoch über
einen anderen Fehler gestolpert.
Auf Startseite der Anwendung kann sich angemeldet werden, sich registriert werden und eine Passwort
zurücksetzten anfrage stellen. über ein Formular kann eine Emailadresse eingetragen werden, an diese
Adresse wird anschließend eine Email versenden.
Diese Email soll einen Deeplink beinhalten der, das Programm öffnet und zur neues Passwort vergeben Ansicht
navigiert.
Im aktuellen Stand des Programm, wurde nur eine Email mit einem Link auf eine andere Internetseite schickt.
Das Ziel meiner Aufgabe war diesen Link zu ändern um um von der erhaltenen Email wieder zurück auf das
Programm zu navigieren.
Beim ersten Testen des Programm um den Ablauf nachzuvollziehen stellte ich jedoch eine Fehler fest und
zwar die Startseite wurde mehrmals aufgerufen.
Während der Fehlersuche konnte ich die Ursache dafür nach und nach eingrenzen indem ich mich mit BloC
(Buissnes Logic components) auseinander setzte um deren Funktionsweise zu verstehen. BLoC ist eine von
vielen State Managementsystem. Das Ziel von BLoC ist es den Code sauber voneinander zu abstrahieren um
die Qualität des Programms zu verbessern. In erster Linie trennt BLoC das Userinterface(UI) von der Logik und
den State von dem Backend. Da BLoC nicht zulässt Funktionen direkt in der UI auszuführen verwendet BLoC
Events. In diesen Events wird ein Identischer State als Eventstate an die Logik weiter gegeben, in der Logik
wird dann die Funktion ausgeführt und anschließend ein neuen State ausgegeben.
Wenn Daten aus der Datenbank abgefragt werden, werden in den Events auch die Abfrage zur Datenbank
separiert definiert und ausgeführt. Dadurch entsteht ein sehr Modulares Programm und es können
verschiedene Aspekte eines Programms geändert werden ohne Einfluss auf andere Teile des Programms zu
haben zb. könnte in dem Event die Logik ganz einfach ausgetauscht werden ohne andere Abschnitte des
Programms zu beeinflussen.
Damit alle teile des Programms mitbekommen wenn neue States übergeben werden, gibt es verschiedene
Widgets die benötigt werden, wie zb. Blocklistener, Blocprovider usw. Nach mehrmaligen lesen des
Programmcodes viel mir auf das mehrere Bloclistener erzeugt wurden. Die Aufgabe eine Bloclistener ist es auf
die Antwort des Events zu warten und darauf zu reagieren. Weil auf Zwei aufeinander folgende Seiten je ein
Bloclistener erzeugt wurde, wurde bei der Funktion der Passwort zurücksetzten Event auch Zwei mal reagiert
und deswegen Zwei mal auf die Startseite navigiert.

&nbsp;
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
