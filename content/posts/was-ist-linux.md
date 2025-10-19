+++
title = "Was ist Linux?"
date = 2025-09-28T09:00:00+02:00
description = "Lerne, wie das Linux-Oekosystem aufgebaut ist und wie sich Distributionen unterscheiden."
summary = "Ein praxisnaher Ueberblick ueber Kernel, Distributionen und die wichtigsten Desktop- sowie Server-Varianten."
level = "Einsteiger"
categories = ["Linux Grundlagen"]
tags = ["kernel", "distributionen", "opensource"]
reading_time = "8 Min"
next_steps = [
  "Installiere eine Linux-Distribution in einer VM oder per WSL",
  "Teste die wichtigsten Terminal-Kommandos mit unserem Cheatsheet",
  "Vergleiche Paketmanager wie apt, dnf und pacman"
]
+++

Linux ist kein einzelnes Betriebssystem, sondern ein flexibles Baukastensystem aus Kernel, Nutzerland und Paketen. Der Kernel stellt Treiber, Speicherverwaltung und Sicherheitsmechanismen bereit. Erst durch Zusatzsoftware wie Shell, Paketmanager, Systemdienste und Desktopumgebungen entsteht eine Distribution.

In der Praxis bedeutet das: Du kannst dir genau das System zusammenstellen, das zu deinem Anwendungsfall passt. Administratorinnen greifen haeufig zu stabilen Server-Distributionen wie Debian oder Rocky Linux. Entwicklerinnen moegen rolling Releases wie Arch Linux, weil neue Pakete schneller verfuegbar sind. Fuer den Einstieg sind Desktop-Distributionen wie Ubuntu oder Linux Mint ideal.

### Komponenten im Ueberblick

- **Kernel:** Grundlegende Hardware-Abstraktion und Sicherheitsfunktionen.
- **Init-System:** Startet Prozesse und Dienste (z. B. systemd, OpenRC).
- **Paketmanager:** Verteilt und aktualisiert Software (z. B. apt, dnf, pacman).
- **Desktop:** Grafische Oberflaeche wie GNOME, KDE Plasma oder Xfce.

> Tipp: Wenn du dir unsicher bist, starte mit einer Desktop-Distro in einer virtuellen Maschine. So kannst du gefahrlos experimentieren.

Weiter geht es mit den ersten Schritten im Terminal, wo du Befehle, Dateisystem und Benutzerrechte kennenlernst.

