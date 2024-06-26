#

| Vorname | Nachname | Beruf               | Dauer       |
| ------- | -------- | ------------------- | ----------- |
| Marten  | Meißner  | Fachinformatiker AE | 07.22-07.24 |
---

## Wochenbericht KW 5.  (2024.01.29. - 02.04.)
---

Da ich bei der Anzahl meiner Provider nicht beschränkt bin, kann ich davon eine große zahl verwenden. Dies ermöglicht mir für viele verschiedene Eigenschaften einen eigenen Provider zu benutzen. So kann ich z. B. ein Sprachenobjekt erstellen und dieses über ein StateProvider auslesen und anpassen.      
Um hier einen gewissen Standard einzuhalten, achte ich darauf, dass der State Provider nur auf Objekte zugreift, die einen Konstanten Konstruktor haben.
Dies erreiche ich dadurch, dass ich zur Klassendefinition das Freezed Package nutzte. Freezed gibt nach außen nur konstante Konstruktoren weiter.
Somit kann das Objekt zur Laufzeit nicht einfach überschrieben werden, sondern muss immer über eine „CopyWith“ Methode ersetzt werden.      
Um bei dem Beispiel der sprach Einstellung zu bleiben, habe ich Settings Objekt, das ein Enum Language hat. Der StateProvider wird angepasst, indem ich z.B. „ref.read(settingsProvider.notifier).state“ auf den State des Providers zugreife und die „copyWith“ Methode aufrufe und dort das Attribute Language anpasse.
In einem weiteren Provider reagiere ich auf die Anpassung des SettingsProvider und tausche dann das Rückgabeobjekt aus, z.B. ändert der Nutzer die Sprache von Englisch auf Deutsch, hier wird das Settingsobjekt angepasst. Dies führt dazu, das im Sprachprovider eine Abfrage ausgelöst und je nachdem welches Enum im Settingsobjekt ausgewählt wird, wird das passende Sprachobjekt im Sprachprovider verwiesen und updatet als Reaktion darauf, alle Wörter in der GUI.       
Somit kann ich für verschiedene wichtige Attribute einen Provider verwenden oder mit überlegen sie weiter zu verkapseln. So kann ein Einstellungsobjekt eine Eigenschaft des Users sein oder selbstständig für die ganze App definiert werden und alle Nutzer teilen sich ein Design.
Eine Liste meiner Provider sind:

    -   ViewProvider
    -   UserProvider
    -   Settingsprovider
    -   DictionaryProvider

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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
