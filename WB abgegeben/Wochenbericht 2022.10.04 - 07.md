#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht 40 .  ( 2022.10.04.- 07.)

Wir haben unsere App unserem Lehrer Vorgestellt und zusammen besprochen was noch nüztliche Funktionen wären.
Eine nützliche Funktion wäre es wenn man das Ganze Produkt über eine eigene Maske anpassen könnte und zusätzlich wäre es praktisch Funktion den "State" zu speichern zu können.
Wir teilten uns in Zwei Teams auf um die Funktione zu Schreiben, dass Eine Team beschäftige sich mit dem erstellen der Funktionen um das Produkt anzupassen und einen weiteren Bildschirm Programmierten in dem es die möglichkeit gibt über GUI Elemente die Eigenschaften des Produktes anzupassen dazu benutzen wir Text Eingabefelder und ein Flutter Package das Filepicker heist, mit diesem Package können Bilder von der Festplatte eingefügt werden und auf dem Smartphone sogar Fotos hochladbar sind.
Ich beschäftigte mich mit der Speicher des "States", dafür las ich Online über Json Datein und das ich mit einer "toJson"Methode, Daten als String auf der Festplatte gespeichert werden kann und mit "fromJson" dieser String wieder umformatieren kann.
Um eine Json (JavaScript Objekt Notation) als String zu speichern werden die Daten in eine Map umgewandelt dazu nutzten wir einen String als Key und wiesen diesem Key dann einen Wert zu. Diese Map wird dann als String gespeichert und kann so als Json Datei verschickt oder gespeichert werden.
Ein Problem war die Umformatierung der Bilder, die können aber als "Base64" String decodierd werden mit der Encode Methode und der Decode Methode wieder zu einen Bild umgewandelt werden.
Um den State zuspeichern brauchte ich einen weiteren Provider, dafür nutzte ich den "Provider Observer" von Riverpod dieser Provider kann mehre "states" verwalten.
der Provider Observer kann den "State" unterscheiden ,dadurch kann ich jedes mal  wenn ein neuer "State" erstellt wird, den neunen "State" registrieren und eine "save" Funktion schreiben die mir den "State" als Json Dokumente speichern.
Wenn ich das Dokument wieder Laden möchte, wird diese "load" Funktion Asynchron da der Computer etwas Rechenzeit braucht und auf eine Antwort meiner Funktion warten muss da die Information nicht im Programm abliegt sonder erst von der Festplatte angefragt werden muss.
Damit ich diese Funktion so durchführen kann muss ich meinem Programm sagen das die Folgende Funktion Asynchron berechnet werden muss und dafür benötige ich das Keywort "async" dadruch weis das Programm das es die Funktion erst ausführen kann wenn die Codezeile mit dem "await" Keywort fertig berechent wurde und damit der Computer in einer Asynchronen Funktion nicht einen Fehler erkennt kann ich ihm dadruch mitteilen das die Funktion nicht normal von Oben nach Unten abgearbeitet werden kann und es zu verzögerungen kommt.
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
