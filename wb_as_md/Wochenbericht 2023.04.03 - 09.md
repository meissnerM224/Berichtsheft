#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 14.  (2023.04.03. - 09.)

---
Nachdem ich mich letzte Woche viel mit BLoC beschäftigte, konnte ich mein Eigentlichen Issue nicht beenden.
Zunächst suchte ich nach dem Blocevent welche aktiviert wird wenn eine Passwortvergessen Anfrage
aufgerufen wird um von dort aus die Logik nachzuvollziehen wie die Einzelnen Schritte sind vom betätigen
der Taste bis hin zum Senden der Email.
Nachdem das Event aktiviert wurde, wird eine Abfrage in der Datenbank getätigt die vergleicht ob die
Angegebene Mailadresse auch zu einem Registrierten Account gehört. Wenn es zutrifft wird eine Email
gesendet, ansonsten werde ich dort eine Nachricht generieren lassen die den Nutzerin darauf hinweist das
dieser noch nicht Registriert ist und dies bitte tun soll.
Alternativ bietet die Datenbank Supabase den Service eine Email mit dem Text sich unter folgenden Link ein
neues Passwort zu erstellen.
Nachdem ich diesen Prozess nachvollzogen habe konnte ich mich darauf konzentrieren wie ich einen Link
erstelle und damit auf meine Anwendung navigiere. Dafür habe ich im Internet recherchiert und viele
Möglichkeiten gefunden die es sehr einfach ermöglichen auf Webseiten oder in Android Apps Links zu
erstellen, doch nicht ganz so einfach war es einen Link für Apple Geräte oder für Pc Anwendungen zu
erstellen.
Um eine Lösung zu finden haben wir verschiedene Programme gesucht die auch so eine Gadget anbieten und
so genannte Deeplinks gefunden. Um ein Deeplink zu erstellen bietet das Framework Flutter eine Libary
Namens "uni_link" an.
Nachdem ich die Libary in die Pubspec.yaml Datei eingebunden habe und diese dann die Aktuellste Version
geladen hat, musste ich zunächst in der "main.dart" Datei die void main Funktion in der das gesamte
Programm läuft mitteilen das diese ab sofort asynchron sein kann und eine Abfrage erstellt die, die Plattform
abfragt ob diese auf einem Windows Gerät läuft?
Wenn dies zutrifft wird im Registerprotokoll auf dem Windows Rechner eine Schnittstelle gespeichert die ich
definieren kann und diese Schnittstelle nutzte ich dann für den Deeplink. Des weiteren musste ich in
verschieden Dateien die für die Windows Version compiliert werden noch implementieren, dass diese auch mit
einem Deeplink aktiveren lässt.
Somit kann ich jetzt Deeplinks für Windows Geräte erstellen und in einer Email versenden.
In den Nächsten Schritte muss nun eine View programmiert werden in der ein neues Passwort erstellt werden
kann und dieses nach Bestätigung des Nutzers dann das alte Passwort überschreibt und eine Bestätigung der
Passwort Änderung eine Email sendet und den Arbeitsschritt bestätigt.
Wenn die "setNewPasswordView" erstellt wurde kann dann der Link um die Navigation dorthin erweitert
werden.

&nbsp;
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
