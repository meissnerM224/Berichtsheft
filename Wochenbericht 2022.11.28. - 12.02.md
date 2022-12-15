#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|FachInoformatiker AE|07.22-07.24|
---

## Wochenbericht KW 48.  (2022.11.28. - 12.02.)

---
Diese Woche habe ich sehr Prakitsch an unserer App gearbeitet und die ganzen neuerungen die wir Impelmentiert haben getestet und refactoring betrieben.
Wir erstellsten einen eigene Klasse für den Datentyp unseres Münzwertes, mit denen der Snackautomat die Funktionen durdchführt, dass hat zur Folge das wir Performanter mit unseren Datentyp arbeiten können als mit einem Primitiven Datentyp der leicht manipuliert ist.
Das hat zur Folge das wir Informationen nicht ausversehen zu einem String oder Intiger deklarieren und diesen dann Falsch weiter benutzen und bei einer null abfrage auch ein null bekommen und nicht eine 0 oder einen Leeren String und dies Zwingt uns bei Jeder Funktion uns mehr mit dem Datentyp zu beschäftigen und somit flüchtigkeits fehler mit zu vermeiden.
zusätzlich Impelementierten wir noch einen weitern Riverpod Provider für unsere  Produkte um unsere Daten menge die wir speichern und updaten zu regulieren, damit nicht jedes mal wenn sich eine einheit anpasst am Produkt einmal alle Datensätze in der App aktualisiert werden, was auf dem Prozessor nicht nicht so viel auswirkung hat, aber wenn wir diese Daten dann auf eine Datenbank laden oder über ein Netzwerk versendet wird, wird doch häufig große Datenmengen ohne wirkliche  auswirkung aktualsiert, was zu Unnötig vielen Daten transfer führt und wartezeiten verursacht.  


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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
