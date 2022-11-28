#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|FachInoformatiker AE|07.22-07.24|
---

## Wochenbericht KW 47.  (2022.11.21.- 25.)

---
Wir bauten unser PHP script um weil es nach mehren Funktionen sehr unübersichtlich war.
Die Befehle haben wir einfach immer untereinander abgefragt was nach Drei abfragen sehr unübersichtlich wurde, deswegen passten wir unser PHP Skript an.
Wir erstellten ein neues PHP "core" Skript was wir mit einer "include" Funktion impelemntieren dadruch müssen wir nur noch die Passwort und Verbindungs Funktion aufrufen die beiden Funktionen haben die Aufgabe Verbindungstestabfrage mit der Datenbank erstellen und eine Funktion mit dessen hilfe wir Informationen der Datenbank manipulieren kann.
Zudem haben wir unsere "http.post()" Methode angepasst.
Vorher haben wir immer unser einzigste PHP Skript aufgerufen und dort eine Branching abfrage nach dem jeweiligen Befehl abgefragt.
Jetzt haben wir eine Basis URL diese enthält die IP Adresse und ist der erste Baustein für unsere URL dazu änderten wir die "databaseResponce" Funktionen diese enthalten keinen Befehl mehr sondern den Scriptname mit der jeweiligen Datenbank anfrage.
Dadurch haben wir unsere Datenkapselung verbessert, weil jetzt jede anfrage ein anderes Script aufruft und Fehler eindeutig aus dieser Funktion kommt und wenn wir änderungen einbauen wollen wird dies nur an einer Stelle anpassen müssen.   
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
