#

| Vorname | Nachname | Beruf | Dauer |
|---|---|---|---|
|Marten| Meißner|Fachinformatiker AE|07.22-07.24|
---

## Wochenbericht KW 29.  (2023.07.17. - 23.)

---
Zu den Struktur Pattern gehören auch noch die Entwurfsmuster der Proxy, Flyweight, Fasade und Composite Pattern.        
Das Flyweight oder Leichtgewicht wird verwendet, wenn häufig ähnliche Objekte erstellt werden, die sich nicht wirklich unterscheiden.       
Dies hat den Vorteil, dass viel Speicher eingespart werden kann, da, hier nicht für jedes Objekt ein vollständiges Objekt erstellt wird, sondern, hier eher nur interne Daten gespeichert werden und mit einem Pointer auf eine andere Speichereinheit verwiesen wird.      
Im Buch Design Pattern wird ein Beispiel genannt, dass ein Text, mit 180.000 Zeichen, mit nur 480 Objekten dargestellt werden kann.     
Weil bei dem Flyweight-pattern nicht jedes Objekt gleicht, wird eine Factory-methode verwendet als Konstruktor, so wird bei jedem Aufruf entschieden. Ist es identisch wie ein schon existierendes Objekt?      
Wenn dies zutrifft, wird in dem Objekt nur positionelle und andere Metadaten gespeichert und mit einem Pointer auf das schon existierende Objekt verwiesen, das sich schon im Cache befindet.       
Wenn es noch nicht existiert, wird ein komplett neues Objekt erstellt.      
Weil das Flyweight Pattern aber nicht so einfach zu implementieren und nicht so leicht zu testen ist, wird häufig nur dann eingesetzt, wenn Ressourcen sparen ein wichtiger Bestandteil ist, der Architektur entscheiden ist.       
Bei den Komposite-Pattern wird versucht komplexe Architektur leichter zu implementieren, indem sich die Objekte rekursive, also sich selbst aufrufend designt werden.       
Mit dem Komposite-Pattern erreicht man eine hohe Flexibilität, Effizienz und eine hohe Abstraktion der Objekte.     
In einem Beispiel mit Angestellten, ist jeder Angestellte ein Mitarbeiter, aber nicht jeder Mitarbeiter ist eine Führungskraft, aber eine Führungskraft ist auch ein Angestellter.      
Im Komposite-Pattern können sich die Composite Objekte sich selber rekursive aufrufen, aber jedes Komposite-Objekt auch gleichzeitig ein Komponente-Objekt.     
So wird mit dem Komposite-Pattern leicht eine Baumstruktur erstellt, so kann jeder Stumpf Äste bilden, diese Äste können weitere Äste bilden und auch Blätter, genauso könne auch am Stumpf Blätter wachsen.   
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
&nbsp;
Kontrolliert am: _________________ Unterschrift  :____________________
