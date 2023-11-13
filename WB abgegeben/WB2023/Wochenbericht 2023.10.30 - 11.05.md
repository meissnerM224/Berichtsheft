#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 44.  (2023.10.30. - 11.05.)

---
Für unser Refactoring Phase startete ich mit dem Umbau des Bauklangobjektes.        
Bisher bekamen wir von der Microsoft ICalendar(.ics) Datei nur eine im JSON formatierte Datei.      
Diese Datei lasen wir mit Regular Expression aus, zerteilten sie und speicherte die Werte der einzelnen Einträge in ein Basis-Datenmodel.       
Da es recht kompliziert war aus der ics Datei direkt ein Datenmodel zu erstellen, entschieden wir uns ein zwischen Datenmodell zu bauen, welches die Logik umfasst, die ics Datei so zu interpretieren, dass wir sie nutzen können.     
Mit diesem Zwischenschritt fiel es uns viel leichte, diese Dateien in Viewmodels zu packen.     
In der ics Datei gibt es eine Eigenschaft rrule(recurrence rule) dieser String enthielt alle Informationen über die Regelung wie ein Termin sich wiederholt.        
Diesen zerteilten wir mit Regular Expression, sodass wir die Regel mit „if-else“ verzweigen Abfragen konnten.       
Da unser Resultat damit funktionierte, aber dennoch nicht sehr performant war, ersetzte ich diese Prozedur mit einer Klasse.        
Ich nannte diese Klasse RRule und gab ihr mehrere Attribute mit.        
Zuerst gab ihr ihre Quelle Information mit, damit es leichter ist Fehler auszulesen.        
Des Weiteren bekam sie eine Eigenschaft „frequenz“, diese nutzte ich ähnlich wie ein Title oder Name, um die Objekte besser zu unterscheiden.       
Des Weiteren bekam sie ein Attribut für Ausnahmen, also für Termine an denen sie durch ein anderes Ereignis blockiert werden.       
Da in dem Quell String „rrule“ sehr effektiv Informationen hinterlegt wird, hab ich meiner Klasse mehrere Attribute gegeben, um dort verschiedene Intervalle wiedergeben zu können, ohne dass sie sich stark unterschieden.     
Der Bauplan für diesen Termin bestimmt die Tage in Wochentagen (Montag-Sonntag), in Monatstag(1,30/31) in welchen Monat(1–12) und zusätzlich nutzt Microsoft noch eine Kombination von Wochentag und Woche im Monat(4Mo).       
Für den letzten Wochentag in einem Monat wird in einer ics Datei auch folgende Abkürzung genutzt (-1SO).        
Diese Informationen ließen sich gut mit einer Regular Expression herausfiltern, gaben aber keine Typsicherheit oder sonstige Optionen.      
Hier merkte ich schnell, dass es sehr viel einfacher und effizienter ist dieses Problem, Objekt-orientiert zu lösen, anstatt es Prozedural abzuarbeiten.        
Im ersten Schritt war es etwas umfangreicher die Klasse zu schreiben, merkte aber schnell wie viel effizienter und einfacher es wurde den rrule String der ics Datei zu bearbeiten und später damit neue Zeitobjekte zu erstellen.      
&nbsp;
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
