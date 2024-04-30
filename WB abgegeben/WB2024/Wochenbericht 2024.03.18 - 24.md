#

| Vorname | Nachname | Beruf               | Dauer       |
| ------- | -------- | ------------------- | ----------- |
| Marten  | Meißner  | Fachinformatiker AE | 07.22-07.24 |
---

## Wochenbericht KW 12.  (2024.03.18. - 24.)

---

Nachdem ich letzte Woche fertig wurde mit der Erstellung der MVP Screens, startete ich diese Woche mit
den ersten API-Aufrufen, der Datenbank. Hierfür wurde ein Termin mit dem Backend Entwickler vereinbart, um den Workflow zu besprechen, wie Daten in die Datenbank transportiert wird oder Informationen von dort geladen werden.        
Um diese Aufrufe testen zu können, nutzten wir den Onlinedienst Postman. Postman visualisiert sehr schön, alle URLs und was dessen Parameter sind. Wie z. B. erstellen eines Zeiteintrags, kann dort eingesehen werden, wie der Backendentwickler die Daten für einen Zeiteintrag erwartet, hier nutzten wir klassisch JSON und in den Fällen, wo Bilder oder andere Medien übergeben werden, nutzen wir Formdata.      
JSON’s haben eine maximale Speichergröße von 59.000 Zeichen. Da Bilder mit normaler Auflösung als Base64 String.
Form Data sind von der Struktur ähnlich wie JSON, sie werden als Key-Value Paare in das Formdata übergeben, nur dass ein Formdata einen viel größeren Speicherbereich als ein JSON. Im Beispiel der MVP können Nutzer ein Bericht über einen Arbeitseinsatz erstellen und diese mit mehreren Bildern bestätigen. Da ein einzelnes Bild mit einer Auflösung von 1024 × 1024 schon zu groß als Base64 in ein JSON zu übersenden. In Dart kann ein Formdata wie eine Liste um einen Map Eintrag erweitert werden. Hier gibt es zwei Methoden einmal „Formdata.fromMap()“ oder „FormData.fields.add()“ für einfache Key, Value Paare wie bei einem JSON. Um Medien in ein Formdata zu speichern, gibt es die Methode „Formdata.files.add()“ in beiden Fällen sollte ein die Datei als ein „MultipartFile“ übergeben werden.     
Die Logik kapselte ich die Riverpod Provider, da zu einem diese nicht von außen aufgerufen werden kann. Aber zum anderen durch Riverpod sehr effizient in die GUI implementiert werden kann. Somit habe ich eine hohe Abstraktion erreicht, was als Resultat einen leicht anpassbaren und verständlichen Programmcode liefert.      
Nach ersten Anfragefehler, die durch Bug auf beiden Seiten gefunden wurden. Konnte nach kurzen Debuggen schnell die Kommunikation zwischen Frontend und Backend hergestellt werden.

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
