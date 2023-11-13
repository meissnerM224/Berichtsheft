#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 46.  (2023.11.13. - 19.)

---
Nachdem in der Viewmodel Klasse die Terminzeit und die Wiederkehregel durch Objekte bzw. durch eine Liste von Zeiten ersetzt wurde.     
Wird jetzt bei dem erstellen einer Termin VM zuerst zwei statische Methoden von der Terminzeit und rrule Klassen aufgerufen diese erzeugen über eine Factory Methode ein Spezielles Regel Objekt, welches alle Erstellung Optionen kennt.       
Anschließend jedoch bevor das zukünftige VM erstellt wird, wird anhand des RRule Objekts alle möglichen Termine für den geben Zeitraum erstellt.        
Durch den Bauplan, der in dem RRule Objekt hinterlegt wird, ist nicht sehr kompliziert eine oder mehre Termine in dem Zeitraum zu erstellen.        
In der Terminzeit Klasse kann ich nun anhand eines Switch Cases schnell herausfinden, in welchem Intervall in diesem Monat Termine stattfinden können.      
Z.b. bei wöchentlichen Terminen kann ich sehr schnell anhand eines assoziativen Arrays herausfinden, welchen Monatstag ich benötige, wenn der vorhandene Bauplan weis das die Termine, die mittwochs stattfinden.       
Das ist es kaum Rechenaufwand in einem Array, in dem der Monatstag und der dazugehörige Wochentag hinterlegt sind.      
Hier kann schnell alle Monatstage zurückgegeben werden, die in ihrem Value Mittwoch stehen haben, so werden die Monatstage, die ein Mittwoch sind fast linear gefunden und erstellt.        
Dadurch dass dem Bauplan auch die Ausnahmen bekannt sind, kann direkt mit beachten werden, wenn ein Termin ausfällt und so werden die mittwochs die ausfallen nicht auch gebaut.        
Da ich die Terminzeiten später separat von den Terminen speichern möchten, benötigen wir noch die ID.       
Wenn für den gewählten Termin in diesem Monat keine Zeitobjekte erstellt wurde, wird für den Termin ein Initial-Termin im Rückgabewert gespeichert und zurück an das Termin VM Objekt weitergeleitet.       
Die in der Liste gespeicherten Zeiten werden, jetzt dem Konstruktor übergeben und dieser erstellt, nun das refactorte Terminobjekt.     
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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
