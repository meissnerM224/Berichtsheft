#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 16.  (2023.04.17. - 23.)

---
Nach dem Light- und Darkmode Feature, baute ich auch gleich noch ein weiteres Feature ein. Für das neue
Feature überlegte ich mir zuerst welche Parameter ich benötige um die Änderung feste mit einem Nutzer
verbinden zu können.
Um den Wert für die Laufzeit aktuelle zu haben brauchte ich also einen weiteres Attribut in dem Appstate,
aber damit dieser auch nach einem Neustart der Anwendung wieder geladen werden kann, muss ich den Wert
auch in die Datenbank speichern.
Um den Wert mit dem jeweiligen Nutzer verknüpfen zu können muss ich mir erstmal Gedanken über die
Datenbank Struktur machen. Um eine Hohe Abstraktion der Datenbank beizubehalten muss ich zudem noch
die Regeln der dritten Normalform einhalten. Dies verlangt das die Information eindeutig und redundant
gespeichert werden.
Da ich mir zusätzlich noch Gedanken über die Datentypen gemacht habe, habe ich auch überlegt wie ich die
Werte in meinem Appstate speichere. Um die Information Atomar abzuspeichern entschied ich mich dafür in
meinem Appstate das Attribute "themeColor" mit dem Type Intiger hinzuzufügen, da dieser Datentyp nach meiner Überlegung am Praktikabelsten ist.
Dieser Type lässt sich sehr einfach zu einem Hexadezimalwert umwandeln und als String in die Datenbank
speichern. Beim Laden des Hex wert kann ich diesen dann sehr einfach in einen Farbwert umwandeln und
eventuelle Fehler abfangen.
Für meine GUI Anwendung habe ich eine Praktische Libary gefunden namens Colorpicker diese ermöglicht
mir sehr einfach eine Farbskala anzeigen zu lassen in dem der Nutzer sehr leicht seine Favorisierte Farbe
auswählen kann. Die Ausgewählte Farbe wird als Hexadezimalzahl gespeichert und in meiner "getThemeData"
Funktion verwenden. Um aus der Ausgewählten Farbe ein Themedata und daraus auch ein Dark- und
Lighttheme zu erstellen, nutze ich das Attribut "farbSchemeSeed", mit diesem Attribute kann Flutter ein
eigenes Farbschema erstellen und direkt Wiedergeben.
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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
