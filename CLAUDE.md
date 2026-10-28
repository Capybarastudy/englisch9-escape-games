# CLAUDE.md – Escape Games für Englisch, Klasse 9 (Realschule Bayern)

Diese Datei liest Claude Code bei jeder Sitzung automatisch. Sie gilt für **alle** Spiele in diesem Repository.

## Wer ich bin und wofür die Spiele sind
- Ich unterrichte Englisch in einer 9. Klasse (Realschule, Bayern), Lehrwerk **Red Line Bayern** (Band 5, Kl. 9).
- Sprachniveau der Klasse: ungefähr **B1**. Klasse 9b, 31 Schülerinnen und Schüler.
- Alle Schüler arbeiten auf **iPads (Safari)**. Gespielt wird in **Teams von 4–5 Personen an einem iPad**, das Schülerbuch liegt offen daneben.
- Die Spiele sind Übungs- und Wiederholungsphasen im Unterricht (ca. 35–45 Minuten), keine Leistungserhebung.

## Technische Regeln (immer einhalten)
1. **Eine einzige Datei:** `games/<thema>/index.html` mit HTML, CSS und JavaScript inline. Keine Frameworks, keine CDNs, keine externen Schriften, Bilder oder Sounds. Das Spiel muss **offline** funktionieren.
2. **iPad zuerst:** muss in Safari auf dem iPad im Hoch- und Querformat (768×1024 und 1024×768) ohne Zoomen und ohne horizontales Scrollen funktionieren. Große Touch-Flächen (mind. 44 px).
3. **Drag & Drop nur mit Pointer Events** (pointerdown/move/up), nicht mit HTML5-Drag-and-Drop (funktioniert auf iOS nicht zuverlässig). Zusätzlich immer eine Alternative per Antippen (erst Karte antippen, dann Ziel antippen).
4. **Fortschritt speichern** in `localStorage` (falls ein Tab neu lädt), mit try/catch abgesichert; das Spiel muss auch ohne localStorage laufen.
5. **Lösungen nicht im Klartext:** Antworten als SHA-256-Hash (crypto.subtle) der normalisierten Eingabe speichern. Normalisierung: Kleinbuchstaben, Leerzeichen am Rand entfernen, mehrere Leerzeichen zu einem, typografische Apostrophe (’) in ' umwandeln. Für den Lehrermodus die Klartext-Lösungen nur verschleiert (z. B. Base64 + XOR) ablegen.
6. **Kein Raten durch Ausprobieren:** falsche Eingabe = Strafzeit (Sauerstoff/Timer −30 s) und kurze Sperre (10–20 s). Rückmeldung bei Mehrfachaufgaben nur als „x von y richtig“, nicht welche Einzelaufgabe falsch ist.
7. **Hinweise:** pro Team begrenzt (z. B. 3 im ganzen Spiel), jeder Hinweis kostet Zeit. Hinweise zeigen auf die **Zeilen im Buch**, verraten aber nie die Lösung.
8. **Lehrermodus:** über `?teacher` in der URL + PIN. Zeigt alle Lösungen, erlaubt Räume zu überspringen und das Spiel zurückzusetzen. Für Schüler ist der Lehrermodus nicht sichtbar.
9. **Datenschutz:** keine Datenübertragung, kein Tracking, keine Analytics. Nur ein frei wählbarer Teamname, keine echten Namen nötig.
10. Keine Konsolenfehler. Funktioniert in aktuellem Safari, Chrome und Firefox.

## Sprache und Didaktik
- **Alles im Spiel ist auf Englisch** (Story, Anweisungen, Hinweise, Rückmeldungen). Klare, kurze Sätze auf B1-Niveau, Wortschatz aus dem Lehrwerk.
- Arbeitsanweisungen eindeutig, mit Verben wie *Read, Match, Put … in order, Type, Tick*.
- **Nicht zu einfach:** Jeder Raum verlangt echtes Textverständnis (Buch S. … mit Zeilenangaben) oder echte Sprachanwendung. Keine Aufgaben, die man ohne Text durch Allgemeinwissen lösen kann. Ablenker (Distraktoren) müssen plausibel sein.
- **Eindeutigkeit:** Jede Aufgabe hat genau eine richtige Lösung. Wo Varianten sprachlich korrekt sind (z. B. *didn't* / *did not*), werden alle akzeptiert.
- **Fakten nur aus den Materialien** im Ordner `materials/<thema>/`. Keine Buchinhalte, Zahlen, Seitenzahlen oder Zeilennummern erfinden. Wenn etwas fehlt: im Code als TODO markieren und mich in der Zusammenfassung darauf hinweisen.
- **Urheberrecht:** Den Buchtext nicht abschreiben. Das Spiel verweist auf „Student's Book p. … , lines …“. Kurze Zitate (max. ein Halbsatz) sind in Ordnung.

## Gestaltung
- Ansprechend, jugendgerecht, nicht kindisch: passendes Farbthema zum Thema, eigene Illustrationen als **inline SVG** (keine Fotos aus dem Internet).
- Eine Story mit Spannungsbogen (Countdown, Räume/Schlösser, Finale), Fortschrittsanzeige (Karte/Raumleiste), Animationen dezent, Ton standardmäßig **aus**.
- Startbildschirm mit Teamname und kurzer Spielanleitung; Endbildschirm mit Urkunde (Teamname, Restzeit, Anzahl Hinweise), die man per Screenshot festhalten kann.
- Wenn die Zeit abläuft: kein „Game over“-Frust, sondern „Time's up – keep going in overtime“ (Weiterspielen mit Kennzeichnung).

## Wenn du ein neues Spiel baust
1. Lies zuerst alle Dateien in `materials/<thema>/` und den Prompt in `prompts/`.
2. Baue `games/<thema>/index.html`.
3. Schreibe `games/<thema>/LOESUNG.md` (Deutsch): alle Räume mit Lösung, Zeilenbeleg, Lehrer-PIN, Hinweise zum Einsatz im Unterricht (Zeit, Teamgröße, Differenzierung).
4. **Teste selbst:** Spiel einmal komplett durchspielen (z. B. mit Playwright), alle Lösungen prüfen, falsche Eingaben prüfen, beide iPad-Ausrichtungen prüfen, Konsole fehlerfrei. Erst dann committen.
5. Verlinke das neue Spiel in `index.html` im Hauptordner (Übersichtsseite aller Spiele).
6. Fasse mir am Ende auf Deutsch zusammen: was gebaut wurde, Link für GitHub Pages, offene Punkte.
