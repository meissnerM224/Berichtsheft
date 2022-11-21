#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|FachInoformatiker AE|07.22-07.24|
---

## Wochenbericht 40 .  ( 2022.10.04.- 07.)

In dieser Woche haben wir unsere App Vorgestellt und zusammen besprochen was noch nüztliche Funktionen wären.
Uns fiel dabei auf das es sehr nützlich wäre wenn man das ganze Produkt über eine eigene Maske anpassen könnte und den "State" zu speichern zu können sehr praktische ist.
Wir teilten uns in Zwei Teams auf um die Funktione zu Schreiben.
Ich beschäftigte mich mit der Speicher Funktion des "States".
Dafür las ich Online etwas über Json und das mit "toJson" Daten als String auf einer Hardware gespeichert werden kann und mit "fromJson" dieser String wieder eingelesen werden kann.
Um eine Json (JavaScript Objekt Notification) als String zu speichern werden die Daten als Map zugewiesen und so als String hinterlegt.
Ein kleines Problem war die Formatierung eines Bildes.
Die können aber als "Base64" String gespeichert werden und mit einer Decode und Encode Methode formatiert werden.
Um den State zuspeichern braucht Riverpod einen weiteren Provider, dafür nutzte ich den "Provider Observer" dieser Provider kann mehre "states" verwalten, der Provider Observer kann in unserer Funktion einen Neuen und einen Alten "state unterscheiden" ,dadurch kann ich jedes mal  wenn ein neuer "state" erstellt wird dies registrieren und eine "save" Funktion schreiben die mir den "state" in Dokumente speichern kann.
Dadurch bekomme ich einen asynchronen Code und nutze "await" und bei der "state" laden funktion eine "readLineSync" was eine Leere Schleife ausführt der den Computer beschäftig bis die Daten bereit sind zur Weiterverarbeitung.
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
Kontrolliert am: ____________________ Unterschrift  : ______________________
