#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 11.  (2023.03.13. - 19.)

---
Nachdem ich Letzte Woche in unserem Projekt "IK_Invetory" mit hilfe von BLoC und anpassung des AppStates
ein Item so angepasst habe das sie nun verwaltbar wurde, habe ich mir für diese Woche vorgenommen ein
"Draggable" Widget in die App zu Programmieren.     
Nach kurzer Online Recherche habe ich herausgefunden das in dem Flutter Framework eine Widget gibt das
ermöglicht ein Element in der GUI anzuwählen und per gedrückt halten von der Ursprünglichen Position zu
einer anderen Position verschieben lässt.       
Um das Widget einzubauen musste ich verschiedene Attribute bestimmen zb. ein feedback Widget zuweisen,
dieses Widget ersetzt dann das angewählte Objekt in der GUI und ermöglicht es eine Drag Animation
anzuzeigen zb. mit einem Icon oder einem neuem Objekt das Identisch zu dem angewählten Objekt
dargestellt werden kann. Zusätzlich musste ich ein data Information zuweisen für spätere Funktionen.
Da ein Objekt so einfach modifiziert werden kann, dass Es gedraggt wird, war es eben so einfach Es als
"DragTarget" zu definieren.     
In dem "DragTarget" Widget gab es verschiedene Funktionen zur Auswahl.      
Zu den Vier Funktionen die zur Auswahl stehen gibt es zusätzlich die Funktion "onWillAccept" hier kann
definiert werden ob das gedraggtes Objekt auch mit dem Zielobjekt interagieren darf.        
Für die Eigentliche Drag Funktion habe ich also ein "Draggable" als auswählbares Objekt markiert und
zusätzlich aber auch als "Dragtarget" aber ohne ein "type" festzulegen, um später auch Items in die Jeweiligen Objekte zuzulassen, definiert.       
Nachdem ich also die Objekte definiert habe musste ich ein BLoC Event schreiben in dem ich das gedraggte
Objekt(data) aktualisieren kann und ihm ein neuen "parent"(child) zuweise. In dem Event wurde auch gleich die Information in der Supabase Datenbank upgedated.      
Dabei bemerkte ich das durch mein Ursprüngliches Event zwar die Node in der Datenbank upgedated wurde aber nicht in der App aktualisiert.       
Um den Appstate auch zu aktualisieren zu können, kann ich einmal nur die Informationen im State neu
zuweisen, aber dies kann unter umständen zu Problemen führen.       
Deswegen entschied ich mich in dem Event nicht nur das ausgewählte Objekt zu aktualisieren sondern auch
die zugehörigen Daten neu aus der Datenbank anzufragen und diese dort hinterlegten Daten mit der "map()"
Methode zu den jeweiligen Datentypen umzubauen und anschließend mit der "toList()" Methode in eine neue
Liste zu formatieren und diese in den State zu speichern.
&nbsp;
\
\
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
