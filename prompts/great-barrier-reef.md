# Prompt für Claude Code: Escape Game „Great Barrier Reef in danger“

Baue ein interaktives Escape Game als **eine einzige HTML-Datei** unter `games/great-barrier-reef/index.html`.

Lies vorher vollständig:
- `CLAUDE.md` (alle technischen und didaktischen Regeln gelten)
- `materials/great-barrier-reef/facts_text2.md` (einzige Faktenquelle, mit Zeilenangaben)
- `materials/great-barrier-reef/vocab_text2.md` (Wortschatz und Grammatik der Unit)
- `materials/great-barrier-reef/lesson_context.md` (was im Unterricht schon gemacht wurde)

## Zielgruppe und Rahmen
- Klasse 9, Realschule Bayern, Red Line 5, Niveau B1. Teams von 4–5 Schülern an einem iPad, **Student's Book pp. 23–24 liegt offen daneben**.
- Spielzeit 40 Minuten. Es soll **anspruchsvoll** sein: Ein durchschnittliches Team soll knapp fertig werden, schnelle Teams brauchen ca. 30 Minuten. Ohne den Text im Buch soll man nicht weiterkommen.

## Story (alles im Spiel auf Englisch)
Titel: **REEF LAB – Escape from the Great Barrier Reef**
Die Schüler sind ein Team junger Meeresforscher in „Reef Lab“, einer Unterwasser-Forschungsstation am Great Barrier Reef. Ein Sturm hat die Station beschädigt, der **Sauerstoff reicht nur noch 40 Minuten** (Timer als Sauerstoffanzeige). Sieben Luken (hatches) trennen sie vom Rettungsboot an der Oberfläche. Jeder Lukencomputer öffnet sich nur, wenn das Team beweist, dass es das Riff versteht. Jede geöffnete Luke gibt einen **Buchstaben** frei. Am Ende ergeben die Buchstaben das Codewort für die letzte Luke.

Ton: spannend, aber nicht beängstigend. Kurze Texte, B1-Englisch.

## Ablauf und Spielmechanik
- Startbildschirm: Teamname eingeben, kurze Anleitung („Open your Student's Book at pages 23–24. You will need it!“), Start-Button.
- Kartenansicht der Station mit 7 Luken + Finale; Luken werden **nacheinander** freigeschaltet.
- Sauerstoffanzeige (40:00, läuft rückwärts). Falsche Antwort: **−30 Sekunden** und 15 Sekunden Sperre („System cooling down …“).
- **3 Hinweise** für das ganze Spiel, jeder kostet **−60 Sekunden**. Hinweise nennen nur die passenden Zeilen bzw. eine Strategie, nie die Lösung.
- Bei Mehrfachaufgaben nur Rückmeldung „x of y correct“, nicht welche falsch ist.
- Gesammelte Buchstaben sind dauerhaft sichtbar (Inventar).
- Wenn der Sauerstoff aus ist: „Emergency oxygen activated – you're in overtime!“ und weiterspielen; die Zeit zählt dann rot weiter.
- Endbildschirm: Urkunde „Reef Rescuers“ mit Teamname, verbleibender Zeit bzw. Overtime, Anzahl der Hinweise; darunter eine offene Reflexionsfrage (nicht bewertet): *"Do we care enough about our earth to protect one of its most beautiful places? Write two sentences."* (Textfeld).

## Die sieben Luken (Inhalte genau so umsetzen)

### Hatch 1 – Word Scanner (Vocabulary) → Buchstabe **O**
Sechs Definitionen; das Team tippt das passende Wort. Zur Hilfe Anzahl der Buchstaben als Striche und der erste Buchstabe.
1. something spectacular – the reef is one of the greatest ___s on earth → **wonder**
2. a community of animals and plants in the same environment → **ecosystem**
3. a sea animal with a hard shell – some come to the reef from the Pacific Ocean → **turtle**
4. the place that you travel to → **destination**
5. to make water, air or land dirty → **pollute** (auch „to pollute“ akzeptieren)
6. the answer to a problem → **solution**
Alle sechs müssen stimmen („x of 6 correct“).

### Hatch 2 – Number Lock (Reading for detail) → Buchstabe **R**
Zahlenschloss mit 4 Rädern. Das Team findet vier Zahlen im Text:
- A = how many kilometres the reef stretches (**2300**)
- B = how many types of coral the text mentions (**350**)
- C = how many kilometres of coral were damaged in 2010 (**3**)
- D = how many million tourists visit the reef every year (**2**)
Code = A + B + C + D = **2655**. Ein Notizfeld für die vier Zahlen anbieten (ohne Prüfung). Hinweis: „Write numbers without commas.“

### Hatch 3 – Chain Reaction (Cause and effect) → Buchstabe **E**
Sieben Karten, davon fünf in die richtige Reihenfolge bringen (Drag & Drop mit Pointer Events + Antipp-Alternative), zwei sind Ablenker:
1. Climate change …
2. The water temperature gets higher.
3. The algae on the coral die.
4. The creatures that need algae for food die.
5. Whole areas of the reef become like ghost towns.
Ablenker: „Seabirds sit on the snorkelling platforms.“ / „A ship goes outside the official lane.“
Textbeleg: ll. 22–33.

### Hatch 4 – Truth Detector (True / False / Not in the text) → Buchstabe **V**
Neun Aussagen, jeweils T / F / NT antippen. Nur „x of 9 correct“ als Rückmeldung.
1. You can see the reef from the moon. → **T** (ll. 8–9)
2. The reef is smaller than the United Kingdom. → **F** (ll. 6–8)
3. Coral bleaching was first seen in the 1980s. → **T** (ll. 24–26)
4. Most of the tourists come from Europe. → **NT**
5. Snorkelling platforms attract seabirds. → **T** (ll. 38–40)
6. The oil spill in 2010 happened because the ship stayed inside the official lane. → **F** (ll. 48–50)
7. Underwater robots help the coral to repair itself. → **T** (ll. 59–61)
8. Australia can stop climate change on its own. → **F** (ll. 62–63)
9. The government has closed the reef to tourists. → **NT**
Vor der Aufgabe kurz erklären: *False = the text says something different. Not in the text = the text gives no information.*

### Hatch 5 – Captain's Logbook (Grammar: simple past, past progressive, used to) → Buchstabe **C**
Ein (ausgedachtes) Logbuch des Kapitäns aus dem Jahr 2010. Das Team tippt die richtige Verbform. Klar kennzeichnen, dass das Logbuch erfunden ist („imagined logbook“).
1. We ___ (travel) through the reef when the ship ___ (go) outside the official lane. → **were travelling** (auch *were traveling*) / **went**
2. While I ___ (look) at the map, the ship ___ (hit) the reef. → **was looking** / **hit**
3. 100 years ago, the coral ___ (be – use *used to*) much more colourful. → **used to be**
4. Before the 1980s, nobody ___ (see) coral bleaching. → **saw** (auch *had seen*)
Insgesamt 6 Lücken. Kurz-/Langformen akzeptieren, Groß-/Kleinschreibung egal.

### Hatch 6 – Threat Map (Reading: threats and measures) → Buchstabe **E**
Teil A: Drei Bedrohungen den Folgen zuordnen (eine Folge ist Ablenker):
- climate change and higher water temperature → coral bleaching
- snorkelling platforms → seabirds' waste pollutes the water
- ships → an oil spill damaged three kilometres of coral
- Ablenker-Folge: „whales leave the reef“
Teil B: „What has the Australian government done? Tick **two**.“
- ✔ It has spent millions of Australian dollars on help for the reef.
- ✔ It has made stricter laws for ships.
- ✘ It has closed the reef to tourists.
- ✘ It has banned all ships from the area.
- ✘ It has built a wall around the reef.
Teil A und B werden gemeinsam geprüft.

### Hatch 7 – Damaged Report (Vocabulary in context) → Buchstabe **R**
Ein beschädigter Bericht mit 7 Lücken. Wortbank mit 9 Wörtern (Wort antippen, dann Lücke antippen; Wörter nur einmal verwendbar).
1. The Great Barrier Reef **stretches** for 2,300 kilometres.
2. Climate change is one of the biggest **threats** to the reef.
3. Warm water causes coral **bleaching**.
4. The waste of seabirds **pollutes** the water.
5. The death of many creatures is a **consequence** of coral bleaching.
6. The **government** has made stricter laws for ships.
7. If no **solution** is found, the reef may be dead by 2030.
Ablenker in der Wortbank: **destination**, **platform**.

### Final Hatch – Codeword
Die gesammelten Buchstaben in der Reihenfolge O R E V C E R. Das Team muss sie zum Codewort ordnen (Buchstabenkacheln verschieben).
Hinweistext: *"What does the reef need many years to do after the oil spill? (p. 23, l. 52)"*
Lösung: **RECOVER**. Danach Ende mit Urkunde.

## Hinweise (je Luke einer, nie die Lösung verraten)
- Hatch 1: „Look at the vocabulary for Text 2 – all the words are in the article.“
- Hatch 2: „The numbers are in lines 4–5, 9–10, 35 and 50–51.“
- Hatch 3: „Read lines 22–33 again. What happens first?“
- Hatch 4: „Check statements 3 and 6 again: lines 24–26 and 48–50.“
- Hatch 5: „Long action → past progressive (was/were + -ing). Short action that interrupts → simple past.“
- Hatch 6: „Look at the headings in the article: Tourists, Ships and oil spills, What can the government do …?“
- Hatch 7: „Read the whole sentence first. Do you need a noun or a verb?“
- Final: „Look at line 52.“

## Lehrermodus
- Aufruf mit `?teacher`, PIN **7193** (gern ändern).
- Zeigt pro Luke die Lösung, Buttons „Skip hatch“ und „Reset game“, sowie eine Übersichtstabelle aller Lösungen zum Projizieren.

## Gestaltung
- Unterwasser-Thema: Blau-/Türkistöne, Korallenfarben als Akzent, Luftblasen-Animation dezent, eigene **inline-SVG**-Illustrationen (Station, Luken, Korallen, Fische, Schildkröte). Keine Fotos, keine externen Dateien.
- Gut lesbar auf dem iPad (Schrift mind. 18 px), hoher Kontrast.
- Wenn eine Luke aufgeht: kurze Animation (Luke öffnet sich) und der Buchstabe „schwimmt“ ins Inventar.

## Zusätzlich erstellen
1. `games/great-barrier-reef/LOESUNG.md` auf Deutsch: alle Lösungen mit Zeilenbelegen, PIN, Einsatz im Unterricht (Teams, Zeit, was die Lehrkraft während des Spiels tut, Auswertung danach).
2. Übersichtsseite `index.html` im Hauptordner mit Link zum Spiel (falls noch nicht vorhanden).

## Qualitätskontrolle vor dem Commit
- Spiel einmal vollständig durchspielen (z. B. Playwright): jede Luke mit richtigen **und** falschen Antworten testen.
- Prüfen: alle Lösungen eindeutig und stimmen mit `facts_text2.md` überein; Antwortvarianten werden akzeptiert; Strafzeit und Sperre funktionieren; Fortschritt bleibt nach Neuladen erhalten; Lehrermodus funktioniert.
- Viewports 768×1024 und 1024×768 prüfen, keine horizontale Scrollleiste, keine Konsolenfehler.
- Danach committen und mir auf Deutsch zusammenfassen, was gebaut wurde und unter welcher GitHub-Pages-Adresse das Spiel erreichbar ist.
