#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|FachInoformatiker AE|07.22-07.24|
---

## Wochenbericht KW47 .  (2022.11.14.- 18.)

---

Ich habe mit hilfe von XAMPP (Microsoft X Apache, MySQL, PHP, Perl) eine Lokale Datenbank erstellt inder ich Informationen unserser Produkte des Snackautomaten eingespeichert.
dann haben wir Methoden entwickelt um mit PHP unsere Informationen aus der Datenbank zu bekommen und Informationen übergeben können.
Ganz nach dem Prinzip der Datenkapselung.
Dadurch reduzieren wir wiederholungen und haben müssen die Logik nicht im ganzen Programm verteilen.
Für die Datenbank abfrage haben wir eine Klasse "Responce" erstellt, Die uns die Datenbank informationen zurückgibt, wir rufen über diese Klasse  unser PHP Programm (Hypertext Prozessor) und diese kommuniziert mit der Datenbank und beinhaltet unsere Abfrage Logik.
Wir stellen in unserer App nur eine Abfrage nach Daten an unsere PHP Datei und wartet ann auf die Antwort, ebenso wartet die Datenbank auf eine Anfrage durch die PHP Anwendung.
Dadurch verwaltet PHP die Logik der Datenabfrage unserer App und der Datenbank.
Dies hat mehre Vorteile einerseits haben wir einen sauberen Code der nicht mit Logik und Funktionen durchzogen ist, was eine Fehlersuche sehr schwer machen kann und dazu enorm schwer zu lesen ist.
Zusätzlich werden sensible Informationen der Datenbank nicht direkt in der App abgerufen und macht es damit Dritten schwer an Daten der Datenbank zukommen.

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
