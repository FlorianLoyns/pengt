# Pengt

**Französisch-Vokabeltrainer mit Karteibox und Leitner-System — eine Single-File-PWA.**

[![Code: MIT](https://img.shields.io/badge/Code-MIT-green.svg)](LICENSE) [![Inhalte: CC BY-SA 4.0](https://img.shields.io/badge/Inhalte-CC%20BY--SA%204.0-blue.svg)](LICENSE-CONTENT.md)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue)](https://florianloyns.github.io/pengt/)
![Keine Abhängigkeiten](https://img.shields.io/badge/Abh%C3%A4ngigkeiten-keine-brightgreen)
![PWA](https://img.shields.io/badge/PWA-offline--f%C3%A4hig-purple)

Eine bunte, mobile Lern-App für Französisch — Karteibox mit Leitner-System, Aussprache per Tastendruck, Combo-Counter, Tagesziel-Ring und Galaxy-Grape-Look.

**[Jetzt lernen](https://florianloyns.github.io/pengt/)**

## Lernprinzip

Eine Karte zeigt vorne ein französisches Wort, hinten die deutsche Übersetzung (oder umgekehrt). Tippen flippt die Karte um. Danach Selbstbewertung über drei Knöpfe: **Wusste nicht** (zurück in Fach 1), **Unsicher** (Fach bleibt), **Wusste ich** (Fach +1, +1 XP).

Karten in Fach 1 wiederholst du am nächsten Tag, in Fach 2 nach 2 Tagen, dann 4, 8 und 16 Tagen. Wer ehrlich bewertet, kommt schneller voran.

## Was die App kann

- **Aussprache per Tap** — Lautsprecher-Symbol auf der Karte spricht das französische Wort vor (Browser-eigene Sprachausgabe, keine Cloud)
- **Combo-Counter** — ab 3× „Wusste ich" in Folge erscheint die Pengt-Pille
- **Tagesziel-Ring** — visuelles Daily-Goal im Galaxy-Gradient
- **Streak-Heatmap** — letzte 30 Tage auf einen Blick
- **XP- und Level-System** — vom Débutant zur Légende
- **Drei Lernrichtungen** — FR→DE, DE→FR oder gemischt
- **Sounds und Haptik** — Web-Audio-Beeps, Vibration, abschaltbar
- **Hell- und Dunkelmodus** — System / Hell / Dunkel
- **Offline-fähig** — PWA, einmal geladen, funktioniert ohne Netz
- **DSGVO-freundlich** — keine Tracker, keine Konten, alles im Browser

## Technisches

Eine einzelne HTML-Datei, kein Build-System, keine Frameworks, keine externen Abhängigkeiten zur Laufzeit. Service Worker für Offline-Cache, `localStorage` für Fortschritt — keine Daten verlassen das Gerät.

## Vokabeln erweitern

In `index.html` nach `const VOCAB = [` suchen und Einträge im Format `["französisch","deutsch"]` ergänzen. Service-Worker-Cache (`sw.js` → `CACHE`-Konstante) nach Änderungen hochzählen, damit der Browser die neue Datei zieht.

## Impressum

Verantwortlich: Florian Loyns. Pflichtangaben nach § 5 DDG und Kontakt: [Impressum](https://florianloyns.com/Impressum/)

## Lizenz

[MIT](LICENSE) für den Quelltext · [CC BY-SA 4.0](LICENSE-CONTENT.md) für die didaktischen Inhalte (Fälle, Fragen, Texte, Grafiken).

Nutzen, anpassen und weitergeben ist ausdrücklich erwünscht — auch im kommerziellen Kontext. Bei den Inhalten gilt: Namensnennung und Weitergabe bearbeiteter Fassungen unter denselben Bedingungen.
