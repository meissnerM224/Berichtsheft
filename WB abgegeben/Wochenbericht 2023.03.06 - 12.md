#
 
| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 10.  (2023.03.06. - 12.)

---
Nach dem Unserer AP1 vorbei war habe ich mich wieder mit unseren Projekt "IK_Inventory" beschäftigt.
Nachdem ich mich wieder in die Programmstruktur eingelesen haben, habe ich mich dafür entschieden ein neues Feature zu Entwickeln.  
In dieser App sollen Items verwaltet werden ähnlich wie bei einer Inventurliste.   
Das Erstellen eines Projektes und darin enthaltene Order und Items wurde schon entwickelt, mein Task für das Feature bestand also darin, die Erstellten Items klickbar zu gestallten und Anschließend auf die "ItemView" weiter zunavigieren.   
Für die Navigation nutzen wir die Push Methode.
Bei dem Navigation wird in Flutter zwischen Benannter und Unbenannet Navigation unterschiedlen.    
Webseiten oder Views in einer App, werden wie ein Stapel bei jeder Push aufruf erstellt die aufgerufenen Seite wird dann einfach vor der Vorheriegen Seite aufgebaut, also beim Starten der App wird die Startseite aufgerufen, wenn von dort aus weiter navigiert wird auf eine andere Seite wird sie darüber erstellt, quasi wie ein Stapel.   
Mit dem Attribute "RouteName", wird eine benannte Navigation aufgerufen, diese wird einmal beim Starten der App oder der Website die benannten Seite in der "App.dart" aufgerufen und erstellt, werden dann bei der Push Navigation über den Aktuellen Screen angezeigt.   
Bei der Unbennaten Navigation wird bei der Navigation eine Build Methode aufgerufen die, Die Seite erst Aufbaut wenn diese Angefragt wird, dadurch könnten eventuell verzögerungen enstehen.
Nachdem ich also das Item Objekt anwählbar war musste sich der State der App anpassen.    
Für die State Verwaltung nutzen wir BLoC(Buissnes-Locig-Component), da BLoc Event´s nutzt um den State zu Aktualisieren musste ich an verschieden Stellen neue Funktionen schreiben und Atributte einfügen, da durch BLoC die Verschiedene Bestandteile der App sehr gut von einander getrennt werden kann und so eine sehr hohe Abstraktion und Modularisierung erreicht werden kann.
So kann eine Anpassung der GUI, der Logik oder der Datenbank ohne größere Hindernisse durchgeführt werden.


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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
