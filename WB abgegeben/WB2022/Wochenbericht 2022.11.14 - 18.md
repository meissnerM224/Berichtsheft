#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW47 .  (2022.11.14.- 18.)

---

Ich habe mit XAMPP (Microsoft X Apache, MySQL, PHP, Perl) eine Lokale Datenbank erstellt in der ich Informationen unserser Produkte des Snackautomaten speichere.
Danach haben wir mit der "http.post" Funktion versucht kontakt mit der Datenbank aufzubauen, dabei lernte ich den Unterschied zwischen "get" und "post" Anfragen.
Die Suchmaschine Google nutzt die get Methode bei ihren Suchanfragen, wenn auf Google was in das Textfeld eingegeben wird, kann auf der Ergebnisseite der Suchtext in der URL gefunden werden, das ist eine häufig benutzte Methode, da mit der get Methode schnell Daten abgefragt werden kann zB.bei Suchanfragen.
Die "post" Methode Funktioniert ähnlich nur das sie einen Body hat und darin die Information hinterlegt wird, dadurch ist die Information nicht direkt in der URL sichbar, dass Erhöt die Sicherheit und vergrößert die Kapazität an Daten die Übermittelt werden können.

Ganz nach dem Prinzip der Datenkapselung haben wir eine Neue Klasse "DatabaseResponce" erstellt, die Klasse dient uns als Schnittstelle zur Datenbank, wenn wir eine Anfrage an die Datenbank senden wollen, rufen wir "DatabaseResponce" auf geben die Anfrage als Json umgewandelt und als Eigenschaft mit.
Wir rufen über diese Klasse  unser PHP Skript (Hypertext Prozessor) und diese kommuniziert mit der Datenbank und beinhaltet unsere Abfrage Logik.
Wir stellen in unserer App nur eine Abfrage nach Daten und unsere PHP Skript und wartet auf die Antwort.
Dadurch verwaltet PHP die Logik der Datenabfrage unserer App.
Dadurch reduzieren wir Wiederholungen und haben die Logik nicht im ganzen Programm verteilen.
Zusätzlich werden Informationen der Datenbank nicht direkt in der App abgerufen und damit schwerer für Unbefugte an Daten der Datenbank zu kommen.

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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
