#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 24.  (2024.06.10 - 16)

---

Diese Woche habe ich hauptsächlich Code Refactoring betrieben.
Mein Hauptaugenmerk waren, die Modellklassen und die Riverpod Provider. Da es hier schon einige nachträgliche Änderungen in der Logik entstanden.
Des Weiteren habe ich mich mit dem Backend besprochen und über die verschieden APIs besprochen und über ein besseres Fehlermanagement geeinigt. Da uns das Backend zu jedem Fehlercode eine Fehlernachricht im HTTP Body übergibt, der den jeweiligen Grund des Abweisens beschreibt. Wie z.B. Typfehler, bei einem Attribute oder wichtige nicht Leer definierbaren Feldern.
Aus diesem Grund habe ich alle CRUD( Create, Read, Update, Delete) Anfragen überarbeitet, da schon die ersten Anfragen nicht mehr aktuell waren und nicht mehr funktionierten. Z.B. änderte sich bei der Post Anfrage zum Erstellen eines neuen Eintrages in die Datenbank, dass die Datenbank im HTTP Header nun einen „Bearer“ Zugangstoken.
Des Weiteren wurde die Logik der übergebenen Daten überarbeitet, da hier z. B. jedes Projekt einzigartig ist und deshalb je einem Kunden zugewiesen werden kann. Dadurch werden die Übergeben-Daten reduziert und bei einem "Man- in-the-Middel" Angriff können die ausgespähten Daten schlechter ausgewertet werden.
Des Weiteren habe ich ein paar GUI Elemente angepasst. Dies hatte zum Ziel den Code leichter lesbarer zu machen. Durch das Auslagern verschiedener Widgets und Methoden in eine Hilfsklasse. Konnten so Aufgaben strikter getrennt werden. Dies reduziert die Logik in den GUI Elementen und Abhängigkeiten.
Dadurch kann der Code flexibel, lesbar und wiederverwendbar werden.

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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
