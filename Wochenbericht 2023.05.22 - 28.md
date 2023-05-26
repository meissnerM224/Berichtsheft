#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 21.  (2023.05.22. - 28.)

---
Nachdem ich Letzte Woche, vorerst das letzte Feature für die IK-Invertory App abgeben habe, habe ich mich mit meinen Mitschüler besprochen und unter Anleitung von Frank als "Teamleiter" für unser Agiles Projekt.
Dadurch übernimmt Frank die Aufgabe einzelne Eckpunkte für unser Projekt zu stecken und uns zu fördern beim Erreichen unserer Ziele.
Dafür wurde ein Projekt bei dem Managmenttool Jira angelegt und erste Issues definiert die im Allgemeinem sich auf dem Erstllen des Grundgerüst der App beziehen, so war zum beipsiel Aufgaben erstellen eines Online Repository auf GitHub um dort unsere Branches und Versionen verwalten zu können.
Desweiteren wurden ersten Issues geplant, wie die Konzipierung des Layouts, des States und Daten die für die App benötigt werden, Erste Oberflächen, das Definieren von Datenmodel Klassen um eine Performantere App zu Entwickeln die mit klarer Struktur und eignen Klassen funktioniert.
Dadurch haben in relativ kurzer Zeit geschafft ein Grundgerüst zu erstellen um im nächsten Schritt uns um Die Datenveraltung kümmern zu können.
Durch die Planung und arbeiten im Team haben wir sehr schnell verschieden Oberflächen erstellen können und an diesen Sogar erste Refactoring betreiben können, so das aus einem einfachen Raster darstellung des Kalenders, jetzt jeder einzelne Tag ein eigens Objekt mit eignen Eigenschaften.
Die einzelnen Kalender kacheln haben wir vorher als eigene Klasse definiert dadurch, kann jeder Tag seine eigenen Attribute erhalten, dies hilft uns dann in den nächsten Schritten Informationen die wir aus einem Datenpaket erhalten ordentlich auseinander zu bauen und die informationen so zu verwalten wie wir sie wiedergeben werden.
Das Ziel ist es externe Kalenderdaten auslesen zu können und diese als Json auf dem gerät zu speichern, so das sie nach einem neustart immernoch vorhanden sind, aber auch so auseinander zunehmen das sie in unsere Daten klassen gespeichert werden können.
Unsere Klassen Struktur planten wir in etwa so, dass ein Jahr eine nummer hat und eine Liste Von Monaten und eine Liste von Wochen beinhalet.
Jede Woche Monat hat eine Liste von Tagen, Jede Woche hat eine Liste von Tagen und eine nummer.
Jeder Tag hat eine Nummer und eine Wochentag nummer, zusätzlich kann jeder eine Liste von Terminen beinhalten.
Diese Struktur macht es uns sehr einfach verschiedene Termine in einem Jahr unhabhängig von ihren Informationen zu hinterlegen und nach Ihren Daten zu sortieren.
Zum Beispiel haben Termine Verschieden Anfangszeiten und Datum, dadurch können wir jeden Termin mit einem Datum einem Tag zuweisen und die Termine nach Uhrzeit sortiert hinterlegen.
Diese Datenstruktur haben wir diese Woche entworfen so das wir jetzt schon einen Funktionsfähigen Kalender gebaut haben, der bis jetzt nur gut aussieht.
In den Nächsten Schritten werden wir uns mit beschäftigen Daten aus dem Internet zu laden und diese so Formatieren, dass die Datei auf dem Computer oder dem Handy gespeichert werden können und anschließend in unseren Kalender integirert werden können.

&nbsp;
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
