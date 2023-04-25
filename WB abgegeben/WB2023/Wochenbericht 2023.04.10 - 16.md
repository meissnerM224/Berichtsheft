#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 15.  (2023.04.10. - 16.)

---
Diese Woche lernte ich viel über den BLoCBuilder.       
Für meine Aktuelle Aufgabe sollte ich eine Erweiterung für das Flutter Framework implementieren.        
Zuerst informierte ich mich Online über die Erweiterung bzw. das Update von Flutter MaterialDesign2 auf MaterialDesign3, also welche änderungen es in dem Update gibt und wie ich es in dem Programm integriere.        
Da in dem Framework Flutter schon Materialdesign aktiv ist musste ich für die Umstellung nur einen Boolwert ändern und schon änderte sich Standard Layout.      
Weil dies so unkomliziert umzusetzen war, dachte ich dran auch gleich ein neues Feature einzubauen, wie eine Einstellmöglichkeit um den Light- und Darkmode zu ändern.      
Nachdem ich mich über die Attributen Thememode und Themedata auseinandersetzte lernte ich, dass diese dazu benutz werden um das Farbschema der benötigt werden und für speichern der Dark- und Lightmode einstellung.
In diesen API´s speichere ich nun Platzhalter Variablen, welche ich in dem State und in der Datenbank hinterlege, damit sie bei dem nächsten start der App auch wieder die gleiche Einstellungen haben wie dem letzten Schließen.
Nach mehrmaliger Code kontrolle und Fehler korrektur, funktionierte mein Feature immer noch nicht, deswegen holte ich mir Frank zur hilfe um gemeinsam nochmal die Architektur des Programms zu analysieren, nach mehrern Logger und Print Anweisung fanden wir herraus, dass Die Feature richtig Funktionierten nur das State Managementsystem baute die Seite nicht neu auf.      
Nachdem wir uns die Listener und die GUI Builder anschauten stellten wir fest, dass die GUI Builder sich nur einmal aufbauen, anstatt bei jeder State änderung die GUI neu aufzubauen.
durch das Attribut "buildWhen" wurde dem BLoC mitgeteilt das dieser sich nicht erneuern soll wenn der State angepasst wird, da es bis jetzt nicht notwendig war.
BLoC besteht aus Vier Hauptbestandteile.
Zuerst gibt es den Controller dieser Kontrolliert die States und teilt den anderen Elemente von BLoC mit das sich etwas getan hat.
Dieser benachrichtigt den Builder, dieser hat nun die Aufgaben die Inforamtionen die im State geändert wurden nun an den Builder weiter zugeben und mit den neuen Werten eine neue GUI aufzubauen.
Damit unser Programm nicht zu viele Daten läd oder unnötig oft aktualisiert haben wir dem "buildWhen" Attribute ein false wert geben damit er nichtmehr sofort neu aufbaut.
Da bei den meisten State änderungen eh eine Seite geladen wird, war es deswegen Sinnvoll den Builder so zu konfigurieren.
Durch das neue Feature wird jetzt aber der State geändert, aber nicht auf eine neue Seite navigiert wird.
Ab jetzt muss der Builder nun doch die aktuelle GUI neu aufbauen, deswegen habe ich in dem "buildWhen" Attribute eine Abfrage gegeben die eine Ausnahme erlaubt wenn sich das State Atribute "bool darkModeActive" in dem neuen State ändert.
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
