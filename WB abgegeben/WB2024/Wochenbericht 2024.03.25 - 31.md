#

| Vorname | Nachname | Beruf               | Dauer       |
| ------- | -------- | ------------------- | ----------- |
| Marten  | Meißner  | Fachinformatiker AE | 07.22-07.24 |
---

## Wochenbericht KW 13.  (2024.03.25. - 31.)

---

Nachdem alle APIs und Funktionen der MVP umgesetzt waren. Begann ich die Woche damit, Tests für Datenmodelle und Logiken zu schreiben.      
Hierfür erstellte ich einen separaten Ordner für Tests in diesem Ordner erstellte ich für die Datenmodelle und für die Provider jeweils eine Datei die „dm_test.dart“ hier testete ich typische Anwendungsfälle ab, die bei der Erstellung eines Objektes auftreten können. Hier könnte ein solcher, falls wie folgt aussehen, jemand versucht einen Zeiteintrag ohne Endzeit oder Nutzer-ID zu erstellen und wie die Klasse bei der Erstellung darauf reagieren würde.     
Ähnlich, aber umfangreicher als das Testen der Datenmodelle war, das Testen der Provider, da hier zuerst eine testbare Umgebung erzeugt werden muss. In Riverpod muss z. b. zuerst ein Providercontainer definiert werden, in dem die Abfrage stattfindet und ausgelesen werden kann. So muss z. B. erst der Providercontainer erzeugt werden, dann muss der Provider mit Daten gefüllt werden und dann können erst die Reaktionen auf die Methoden vergleichen zu können.      
Nach ausführlichen Unit-Tests wurde nochmal ein Funktionstest mit dem Projektleiter durchgeführt. Was die letzte Abnahme war, um die Userstorys im Jiraboard abzuschließen.     
Diese Woche schloss ich die dritte Projektphase, das Implementieren und Testen der MVPs.


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
