#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 48.  (2022.11.28. - 12.02.)

---
Wir haben diese Woche wieder unsere App umgebaut, die Ganzen Neuerungen die wir Implementiert haben wir mit Unit Test getestet und Refactoring durchgeführt.
Wir erstellen eine Eigenen Datentyp der Unserere Münzen darstellt, mit denen der Snackautomat Funktionen durchgeführt, dass hat zur Folge das wir Performanter mit Unseren Datentyp arbeiten können, als mit einem Primitiven Datentyp wie String oder Integer die leicht manipulierbar sind.
Das hat zur Folge das Informationen nicht Ausversehen zu einem String oder Integer deklariert werden und diesen dann Falsch weiter benutzt werden und bei einer "null" Abfrage auch ein "null" bekommen und nicht eine 0 oder einen Leeren String, dass Zwingt uns bei Jeder Funktion mehr mit dem Datentyp zu beschäftigen und somit flüchtigkeits Fehler zu vermeiden.
zusätzlich Implementierten wir noch einen weitern Riverpod Provider für unsere Produkte um unsere Datenmenge die Gespeichert oder upgedatet wird zu regulieren, damit nicht jedes mal wenn sich eine Eigenschaft anpasst am Produkt einmal alle Datensätze in der App aktualisiert werden.
Was auf dem Prozessor nicht so viel Auswirkung hat, aber wenn wir Diese Daten dann immer und immer wieder auf eine Datenbank laden oder über ein Netzwerk versendet wird, wird doch häufig Große Datenmengen ohne Auswirkung Aktualsiert, was zu Unnötig vielen Datentransfer führt und Wartezeiten verursacht.


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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
