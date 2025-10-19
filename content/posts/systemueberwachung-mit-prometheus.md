+++
title = "Systemueberwachung mit Prometheus"
date = 2025-10-18T14:15:00+02:00
description = "Richte Prometheus und Node Exporter ein, definiere Alerts und visualisiere Kennzahlen mit Grafana."
summary = "Ein End-to-End Walkthrough fuer Observability auf Linux-Servern inklusive Beispiel-Dashboards."
level = "Professional"
categories = ["Monitoring"]
tags = ["prometheus", "grafana", "observability"]
reading_time = "18 Min"
next_steps = [
  "Installiere den Node Exporter auf zwei Hosts und vergleiche Metriken",
  "Richte individuelle Alert-Regeln fuer CPU, RAM und Filesystem ein",
  "Verknuepfe Prometheus mit Slack oder Teams fuer Benachrichtigungen"
]
+++

Monitoring wird ab einer gewissen Infrastruktur-Groesse unverzichtbar. Prometheus sammelt Metriken per Pull-Modell, speichert sie effizient und stellt eine Query-Sprache (PromQL) bereit.

```bash
# Prometheus als Service installieren (Beispiel Debian/Ubuntu)
sudo useradd --no-create-home --shell /bin/false prometheus
sudo mkdir -p /etc/prometheus /var/lib/prometheus
```

Wir gehen Schritt fuer Schritt durch die Konfiguration, bauen einen ersten Alert und spielen ihn via Alertmanager aus. Anschliessend verbinden wir Prometheus mit Grafana, um Dashboards fuer Infrastruktur-Teams bereitzustellen.

> Best Practice: Dokumentiere Alerts mit Erwartungswert und Runbook, damit On-Call-Teams effizient reagieren koennen.

Im Downloadbereich findest du Beispiel-Dashboards sowie Playbooks fuer Incident Response.

