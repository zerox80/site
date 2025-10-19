+++
title = "Terminal-Grundlagen: Arbeiten mit der Shell"
date = 2025-10-05T10:30:00+02:00
description = "Die wichtigsten Shell-Konzepte, Befehle und Tastenkombinationen auf einen Blick."
summary = "Uebe Navigationsbefehle, Ausgabeumleitungen und Tastenkombinationen, um dich im Terminal sicher zu bewegen."
level = "Einsteiger"
categories = ["Linux Grundlagen"]
tags = ["shell", "navigation", "alias"]
reading_time = "12 Min"
next_steps = [
  "Richte dir Aliases und Funktionen in deiner .bashrc ein",
  "Experimentiere mit Pipes, um Kommandos zu verketten",
  "Nutze die History effizient mit reverse search (Ctrl+R)"
]
+++

Die Shell ist deine direkte Schnittstelle zum System. Mit ein paar Kernbefehlen navigierst du schnell durch Verzeichnisse, bearbeitest Dateien und kombinierst Kommandos.

```bash
pwd            # aktuelles Verzeichnis anzeigen
ls -lah        # Dateien mit Details und versteckte Eintraege listen
cd projects    # in ein Verzeichnis wechseln
mkdir -p logs  # Verzeichnisstruktur anlegen
rm -rf tmp     # Inhalte rekursiv loeschen
```

Ein solides Gefuehl fuer die Shell entwickelt sich durch wiederholtes Ueben. Nutze unseren Befehlstrainer, um Fehlermeldungen direkt auszuwerten und deine Loesung anzupassen.

### Tastenkombinationen, die du kennen solltest

- `Ctrl + A` und `Ctrl + E` springen zum Anfang bzw. Ende der Zeile.
- `Ctrl + U` loescht den kompletten Eingabetext, `Ctrl + W` nur das Wort links des Cursors.
- `!!` fuehrt den letzten Befehl erneut aus, `!sudo` wiederholt ihn mit `sudo`.

Durch `man <kommando>` oder `kommando --help` findest du zu jedem Tool weiterfuehrende Beispiele. Unsere Cheatsheets bieten passende Zusammenfassungen zum Download.

