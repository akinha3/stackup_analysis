# Stackup Analysis Dashboard

Interaktives 1D-Toleranzanalyse-Dashboard für mechanische Toleranzketten mit:

- Worst Case (WC)
- RSS (Root Sum Square)
- Monte Carlo Simulation
- Virtual Manufacturing KPIs (Cpk, Ausschuss in ppm)
- Sensitivität als Tornado/Pareto

## Features

- Eingabe mehrerer Bauteile mit `Nenn`, `Tol+`, `Tol-`
- Zielgrenzen `LSL` / `USL`
- Simulationsmodi: Uniform, Gauss (truncated), Legacy Truncated Normal
- Live-Visualisierung:
  - Stackup-Balken (Target vs WC vs RSS vs MC)
  - Histogramm
  - Tornado-Diagramm
- PDF/Print-Ansicht mit hoher Lesbarkeit
- Lokales Speichern/Laden per LocalStorage

## Nutzung

1. `index.html` im Browser öffnen.
2. Bauteile und Toleranzen eingeben.
3. Optional Zielgrenzen (`LSL`, `USL`) setzen.
4. `Berechnen` oder `Simulation starten (10k Runs)` ausführen.

## Hinweise

- Einheit: mm
- `Tol+` und `Tol-` als positive Beträge eingeben
- Für gültige Zielgrenzen gilt: `LSL < USL`

## Deployment auf GitHub Pages

Wenn `index.html` im Repository-Root liegt:

1. Repository öffnen → **Settings**
2. **Pages** → **Build and deployment**
3. Source: **Deploy from a branch**, Branch: **main**, Folder: **/(root)**

Danach ist die Seite typischerweise erreichbar unter:

`https://akinha3.github.io/stackup_analysis/`
