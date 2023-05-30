#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 21.  (2023.05.22. - 28.)

---
Nachdem ich letzte Woche vorerst das letzte Feature für die IK-Invertory App abgeben habe, habe ich mich mit meinem Mitschüler besprochen und unter Anleitung von Frank als "Projektleiter" für unser agiles Projekt.
Dadurch übernimmt Frank die Aufgabe einzelne Eckpunkte für unser Projekt zu stecken und uns zu fördern beim Erreichen unserer Ziele.
Dafür wurde ein Projekt bei dem Managementtool Jira angelegt und erste Issues
definiert, die im Allgemeinen sich auf dem Erstellen des Grundgerüstes der App beziehen, so war zum Beispiel Aufgaben erstellen eines Online Repository auf GitHub, um dort unsere Branches und Versionen verwalten zu können.
 Des Weiteren wurden ersten Issues geplant, wie die Konzipierung des Layouts, des States und Daten, die für die App benötigt werden, erste Oberflächen, dass Definieren von Datenmodel Klassen, um eine performantere App zu entwickeln, die mit klarer Struktur und eignen Klassen funktioniert. Dadurch haben in relativ kurzer Zeit geschafft ein Grundgerüst zu erstellen um im nächsten Schritt uns um die Datenverwaltung kümmern zu können. Durch die Planung und arbeiten im Team haben wir sehr schnell verschieden Oberflächen erstellen können und an diesen sogar erste Refactoring betreiben können, sodass aus einer einfachen Rasterdarstellung des Kalenders, jetzt jeder einzelne Tag ein eigens Objekt mit eignen Eigenschaften ist. 
Die einzelnen Kalender kacheln haben wir vorher als eigene Klasse definiert dadurch, kann
jeder Tag seine eigenen Attribute erhalten, dies hilft uns dann in den nächsten Schritten Informationen, die wir aus einem Datenpaket erhalten, ordentlich auseinander zu bauen und die Informationen so zu verwalten, wie wir sie wiedergeben werden. Das Ziel ist es externe Kalenderdaten auslesen zu können und diese als JSON auf dem Gerät zu speichern, sodass sie nach einem Neustart immer noch vorhanden sind, aber auch so auseinander
zunehmen, dass sie in unsere Datenklassen gespeichert werden können. 
Unsere Klassenstruktur planten wir in etwa so, dass ein Jahr eine Nummer hat und eine Liste von Monaten und eine Liste von Wochen beinhaltet.
Jeder Monat hat eine Liste von Tagen, jede Woche hat eine Liste von Tagen und eine Nummer. Jeder Tag hat eine Nummer und eine Wochentag-Nummer, zusätzlich kann jeder eine Liste von Terminen beinhalten.
Diese Struktur macht es uns sehr einfach verschiedene Termine in einem Jahr unabhängig von ihren Informationen zu hinterlegen und nach Ihren Daten zu sortieren. Zum Beispiel haben Termine verschieden Anfangszeiten und Datum, dadurch können wir jeden Termin mit einem Datum, einem Tag zuweisen und die Termine nach Uhrzeit sortiert hinterlegen. Diese Datenstruktur haben wir diese Woche entworfen, sodass wir jetzt schon einen funktionsfähigen Kalender gebaut haben, der bis jetzt nur gut aussieht. 
In den nächsten Schritten werden wir uns mit beschäftigen, Daten aus dem Internet zu laden und diese so formatieren, dass die Datei auf dem Computer oder dem Handy gespeichert werden können, um sie anschließend in unseren Kalender zu integrieren.

&nbsp;
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
