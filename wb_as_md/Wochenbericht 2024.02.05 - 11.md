#

| Vorname | Nachname | Beruf               | Dauer       |
| ------- | -------- | ------------------- | ----------- |
| Marten  | Meißner  | Fachinformatiker AE | 07.22-07.24 |
---

## Wochenbericht KW 6.  (2024.02.05. - 11.)

---
Für eine Profilübersicht wollte ich den Nutzern ermöglichen, das Profilbild anzupassen zu können. Hierfür nutze ich das FilePicker Package. Mit dem FilePicker kann auf verschiedene Hardware zugegriffen werden, wie z.B. Kameras, Bilderverzeichnis oder andere Medienquellen.        
Als Rückgabewerte bekomme ich ein "XFile". Ein XFile ist ein Medium (Bilder, Videos, Audio, Text), das nur im RAM existiert ist und ohne weiter Aktionen direkt gelöscht wird. Um es lokal speichern zu können, muss ein Speicherort festlegen werden. Hierfür nutze ich das "path_provider" package, welches mir die Arbeit abnimmt, einen Speicherort manuell zu suchen und gibt mir z.B. unter Windows den Dokumentenpfad für das Dokumentenverzeichnis.     
Wen ich nun ein Bild mit der Kamera erstelle, bekomme ich ein XFile. Um dieses XFile in ein einfaches File zu konvertieren, benötige ich ein Speicherort, an dem die File Bytes gespeichert werden sollen. Dieses erstelle File kann ich in den Firebase Blob Storage hochladen, als Antwort erhalte ich eine Firebase-Url, die ich einem Userobjekt speichern kann. Dadurch erhalte ich ein schlankes Datenmodell, bei dem ich nicht immer die Bilddaten mit übergeben muss.       
Für die GUI nutze ich einfach das Image Widget. Für den Fall, dass der Nutzer noch kein eigenes Bild hinterlegt hat, erstelle ich alle Nutzerobjekte mit einem Standardbild, dieses kann der Nutzer austauschen durch ein individuelles erstelltes Bild.        
Prinzipielle gibt es für die Gerätehardware erhöhte Sicherheitsmaßnahmen, die mir den Zugriff ablehnen. Hierbei hilft mir das "permisson_handler" Package.
Das Package erlaubt die Einsicht auf die Zugriffsberechtigung des Gerätes. Mit diesen Informationen kann ich darauf reagieren, wenn z. B. der Nutzer mir den Zugriff nicht gewährt hat und kann ihn dann drauf hinweisen, dass er mir dies erlaubt.     
Falls er es abgelehnt hat. Kann ich darauf reagieren und kann den Nutzer ein Pop-up anzeigen, das ihn darauf hinweist, in den Einstellungen die voreingestellten Einstellungen anzupassen, damit z.B. ein Bild aus dem Speicher geladen werden kann oder mit der Kamera ein neues Bild erstellt werden kann.

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
