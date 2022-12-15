#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|FachInoformatiker AE|07.22-07.24|
---

## Wochenbericht KW 49.  (2022.12.05. - 09.)

---
Ich hab sehr Viel Zeit verwendet um Mich in PHP einzuarbeiten, da wir unsere Datenbank Abfrage schon recht Gut funktionierte, aber leider noch viele Bugs aufwies.
Zum Beispiel wurden unsere Produkte des Snackautomaten mit ihren Indexwerten unserer Liste "SlotContent" abgerufen und auch gespeichert, immer wenn ich also keinen ausgewähltes Produkt in der Datenbank Hinterlegen wollte habe ich dafür die Zahl des Jeweilien Index in die Datenbank gespeichert also eine Zahl zwischen 0-8, in Unserem Snackautomaten haben wir für ein nicht ausgewähltes Prodkut immer den wert null(einen nichts Wert) in den State gespeichert.
Wenn ich also diesen Wert in die Datenbank übergeben möchte muss das PHP skrip unterscheiden ob ich eine Null(0) oder ein null(den nichts Wert) einspeichern möchte.
Bis dahin hat unserer Programm einen String 'null' gespeichert, was zu folge hatte das wenn wir den Wert abfragten uns die Datenbank aber den Intiger 0 zurück gab, dies hatte keine Fehler ausgerufen, zeigte aber das wir unsere Daten nicht Richtig abspeicherten.
Deswegen habe Ich mich viel über PHP informiert, über Daten Typen und null Safty.
Im PHP Skript nutze ich dann für Alle Werte die ein "null" enthalten können eine "if (!isset())" abfrage durch alternativ hätte Ich auch "is_null()" funktion verwenden können, dadruch konnte ich mich vergewissern das eine Variable wirklich den Wert "null" enthält und nicht die Zahl 0 bzw. unsere Variablen Strings enthalten "0" enthält.
Desweitern lernte ich das in PHP mehrere Optionen gibt einen SQL befehl zu übermitteln gibt, wir nutzen die Funktion "mysqli" alternativ gibt es noch die Funktion "PDO" mit der ich zb in Dart eine "try catch" Funktion einsetzten die versucht die Datenbank Antowrt umsetzen auch wenn sie Fehlerhaft ist und eine besseres Error Managemend hat.
In der "mysqli" Funktion habe ich zusätzlich alle Update Variablen in Anführungszeichen gesetzt, dies hat zur Folge das alle Variablen als String in die Datenbank Übergibt und dadurch selbst wenn ich ein null wert übergeb sie als String "Null" gespeichert wird und so auch abgerufen wird, zur Lösung habe ich die Variablen, Die die Informationen des Snackautomaten enthalten nicht mehr in Anführungszeichen gesetzt, wodurch die Informationen auch so übergeben wurden wie ich sie Angebe und werden nicht in der "myscli" Funktion in einen String übergeben.
Dadurch übergab ich meine Informationen auch in dem Typ in dem ich sie Definierte.
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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
