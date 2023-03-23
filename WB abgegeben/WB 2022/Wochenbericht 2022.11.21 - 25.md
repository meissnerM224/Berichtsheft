#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 47.  (2022.11.21.- 25.)

---
Wir bauten unser PHP Skript um weil es nach mehren Funktionen sehr unübersichtlich war.
Die Befehle wurden einfach immer untereinander abgefragt was nach Drei abfragen sehr unübersichtlich wurde, deswegen passten wir unser PHP Skript an.
Wir erstellten eine neue PHP "core" Skript was wir mit "include" implemntieren dadruch müssen wir nicht mehr die Passwort und Verbindungs abfragen. Die Funktion "Verbindungstestabfrage" mit der wir die Datenbank aufrufen und eine Funktion mit dessen hilfe wir Informationen der Datenbank manipulieren kann.
Zudem haben wir unsere "http.post()" Methode angepasst.
Vorher haben wir immer unser einzigstes PHP Skript aufgerufen und dort nach eine branching Abfrage nach dem jeweiligen Befehl abgefragt.
Jetzt haben wir eine Basis URL diese enthält eine IP Adresse und ist der erste Baustein für unsere URL dazu änderten wir die "databaseResponce" Funktionen diese enthalten nicht mehr das Schlüsselwort nach dem die If abfragen unterscheiden, sondern den Skriptname mit der Jeweiligen Datenbankanfrage.
Dadurch haben wir unsere Datenkapselung verbessert, weil jetzt jede Anfrage ein anderes Skript aufruft und Fehler eindeutig aus dem Jeweiligen Skript kommt und wenn wir änderungen implementieren werden wir dies nur an einer Stelle anpassen müssen.   
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
