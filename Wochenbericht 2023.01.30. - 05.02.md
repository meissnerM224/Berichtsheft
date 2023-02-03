#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 5.  (2023.01.30. - 02.05.)

---
Durch die Vorbereitung der Zwischenprüfung haben wir uns mit Festplatten und Datensicherung beschäftigt.
In der Datensicherung gibt es unterschliche Speicherverfahren auch als Raidsystem bekannt, es gibt Sechs unterschiedliche Raid level 0,1,5,6,10,01.     
Dabei habe ich mir Folgende Eselbrücke gemerkt, dass Raidlevel bezieht sich auf die Speicherung bei level 0(oder Striped) gibt es "0" Kopien, aber erhöhte Speichergeschwindigkeit da für Raidsystem mind. 2 Festplatten benötigt werden.       
bei Raidlevel '1' gibt es "Eine" vollständige Kopie aller Daten, was praktisch ist weil man Zwei unabhänige Festplatten hat und somit eine Festplatte als Sicherung übrig bleibt. 
Das hat aber mehrere Nachteile zb. wird langsamer die Daten gespeichert weil alle Daten Doppelt gespeichert werden und es wird Doppelt so viel Speicher verbraucht(Redundanz).      
Das Spannenenste Raidsystem ist das Raidlevel 5, hier werden mind. 3 Festplatten benötigt, auf Zwei Festplatten kann Parralel die Daten gespeichert werden und auf der Dritten Festplatte wird mit einer XOR Prüfverfahren eine Prüfsumme erstellt, dieser Prüfsumme kann dann jede Kombination der Daten wiederhergestellt werden wenn "Eine" Festplatte Kaputt geht als Beispiel es gibt eine Festplatte die "1111" und aud der Zweiten Festplatte ist "0000" auf der Dritten wird die Prüfsumme "1111" gespeichert, wenn jetzt die Erste Festplatte mit dem Wert "1111" kaputt geht hat die Prüfsummen Festplatte den passenden gegenwert gespeichert, wenn die Zweite Festplatte kaputt geht Kann mit einer XOR rechnung das Ergebniss wieder errechnet werden zB. "1111" und "1111" ergibt "0000" weil im Binärsyste, nur von 0 bis 1 gerechnet werden kann, also wenn wir 1+1 rechnen ist das Ergebniss = 0 und einen Übertrag von 1.
Dadurch haben wir den Vorteil das mind. Zwei Festplatten gleichzeitig im Striped verfahren beschrieben, wie im Raidlevel 0, auch eine Datensicherung wird erstellt und benötigt nur 33% mehr Speicher, aber Raid 5 funktioniert mit beliebig vielen Festplatten, dabei sinkt für Jede zusätzliche Festplatte die Menge der Redundanz. Dadurch wird eine gute Schreibperformance erzeugt, mit wenig zusätzlichen mehr Speicher kann der Verlust von einer Festplatte kompensiert werden.
Das Raidlelvel 6 Funktioniert ähnlich nur das es hier Zwei Prüfsummen erstellt werden und dadurch der Verlust von Zwei Festplatten Kompensiert werden kann.     
Im Raidlevel.10 werden zwei Lösungswege angestrebt, einmal die Lösung des Raid.1 und die des Raid.0, 
es wird auf 4 Festplatten geschrieben (level.0) also im Striped verfahren, aber jede Information wird auf mind. 2 Festplatten abgespeichert. Dadurch kann wie im Raid.0 verfahren die informationen auf zwei Festplatten aufgeteilt und zusätzlich eine Kopie auf einer jeweils weiteren geschrieben.
Raid 01 ist die umgekehrte Reiehenfolge vom Raid.10 system.

&nbsp;
\
\
\
\
\
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
