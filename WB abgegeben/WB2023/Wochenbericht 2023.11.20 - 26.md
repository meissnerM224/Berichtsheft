#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 47.  (2023.11.20. - 26.)

---
Nachdem Umbau der Datenlogik, ist die Implementation der neuen Datenklassen etwas mehr denk Arbeit gewesen,
aber die Organisation der Datenstruktur viel effektiver.        
Da unsere Viewmodel nun mehr Logik bekommt, wird dadurch der Aufruf und das Erhalten der gewünschten Informationen etwas umständlicher, dafür wurde die Erstellung der VM’s in sich verschachtelt und gibt uns für den gewünschten Zeitraum alle möglichen Termine zurück.      
Z.B. wenn aus einem Datenmodel ein Vievmodel gebaut wird, baut das VM zuerst ein RRule Objekt, welches den Bauplan für wiederkehrende Termine enthält.      
Wenn das VM inzwischen ein RRule Objekt gebaut hat, nutzt sie diese im nächsten Schritt, um Termine im gewählten Zeitraum zu validieren und dann eine Liste von Terminzeiten zurückzugeben.     
Wenn also ein VM aus einer DM gebaut wird, wird zuerst ein Regel-Objekt erstellt und basierend auf dem Regel-Objekt alle Zeiten ermitteln.      
Anschließend dabei berücksichtigend, ob die Terminserie noch aktuell ist und ob es Ausnahmen Regelungen gibt,
wie z. B. ein Termin fällt aus wegen Urlaub.        
Nachdem die ganze Erstellungslogik nun in die Objekte selber implementiert wurden, ganz wie es im Buch der Group of Four (Design Pattern) ist es nun sehr einfach in einem Event, alle möglichen Termine für einen Monat zu erhalten.       
Da jedoch jedes Termin VM auch eine Liste von Zeiten enthält, ist es inzwischen auch sehr einfach, die Termine aus den VM’s in eine Map zu speichern.       
Indem ich meiner Map abfrage, ob es einen Schlüssel gibt, der gleich ist wie mein Startdatum, wenn dies zutrifft, wird dem Value dieser Map zusätzlich zu den vorhandenen Terminen jetzt auch dieser Termin hinzugefügt.        
Inzwischen wurde mein Programmcode nicht nur leichter lesbar, sondern auch noch effizienter geschrieben, da hier nur einmal Termine erstellt werden, diese nur noch die Daten enthalten, die benötigt werden und keine Doppelung von Daten.     
Außerdem muss jetzt nicht mehr in einer Liste Termine, die Termine finden, sondern kann direkt über den Key auf alle Termine zugreifen zu dem gewünschten Tag.      
Zusätzlich kann ich nun auch rekursive die Terminzeiten für einen Monat in der Vergangenheit und der Zukunft  laden, um nicht während der Navigation, anzufangen alle Termine neu zu erstellen.     
In der App wird inzwischen immer die Terminzeiten für den jeweiligen Tag abgefragt, dies geschieht jetzt linear, da jetzt über den Key direkt der richtige Value gefunden werden kann.      
Anders als in einer Liste, in der ich alle Objekte abfragen muss und ich frühsten aufhören kann, wenn ich das gewünschte Objekt gefunden habe.      
&nbsp;
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
