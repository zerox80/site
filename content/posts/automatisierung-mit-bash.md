+++
title = "Automatisierung mit Bash: Aufgaben planen"
date = 2025-10-12T08:45:00+02:00
description = "So baust du wiederverwendbare Bash-Skripte, setzt Variablen sinnvoll ein und planst Jobs mit cron."
summary = "Schreibe robuste Skripte mit Funktionen, Logging und automatisierten Checks – inklusive Cronjob-Vorlagen."
level = "Fortgeschritten"
categories = ["Automatisierung"]
tags = ["bash", "cron", "scripting"]
reading_time = "15 Min"
next_steps = [
  "Erstelle ein Skript, das Logs rotiert und archiviert",
  "Nutze cron und systemd timers fuer regulaere Aufgaben",
  "Setze Shellcheck ein, um Skripte statisch zu analysieren"
]
+++

Automatisierung spart dir Zeit und reduziert Fehlerquellen. In diesem Guide lernst du, wie du Bash-Skripte strukturierst, Eingaben pruefst und mit Exit-Codes umgehst. Wir nutzen `set -euo pipefail`, um typische Stolperfallen abzufangen.

```bash
#!/usr/bin/env bash
set -euo pipefail

log() {
  printf '[%(%Y-%m-%d %H:%M:%S)T] %s\n' -1 "$1"
}

require() {
  command -v "$1" >/dev/null 2>&1 || {
    log "Fehlendes Kommando: $1" >&2
    exit 1
  }
}

require tar
require gzip
```

Mit Funktionen kapselst du wiederkehrende Aufgaben. Kombiniere das mit Parameter-Parsing (`getopts`), um Skripte flexibel zu machen. Der Artikel enthaelt eine Vorlage, die du fuer Backup-Jobs, Log-Rotation oder Wartungsskripte anpassen kannst.

### Cronjob-Blueprint

```cron
0 3 * * * /usr/local/bin/backup.sh >> /var/log/backup.log 2>&1
```

Uebertrage das Konzept auf `systemd`-Timer, um Abhaengigkeiten und Healthchecks komfortabel zu definieren.
