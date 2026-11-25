# tinymd-cpp

Ein kleines Lernprojekt, um C++ (C++20) zu lernen. Ziel ist ein schlanker
**Velocity-Verlet-Integrator** zum Lösen von **Molekulardynamik-Simulationen (MD)**.

Der Schwerpunkt liegt auf sauberem, verständlichem Code und dem Erlernen moderner
C++-Konzepte, nicht auf maximaler Performance oder Vollständigkeit.

## Bauen

Voraussetzungen: CMake ≥ 3.20 und ein C++20-fähiger Compiler.

```powershell
cmake -S . -B build
cmake --build build
```

## Meilensteine

### 1. Velocity-Verlet-Integrator
- [ ] Grundlegende Datenstrukturen: 3D-Vektor, Teilchen (Position, Geschwindigkeit, Kraft, Masse)
- [ ] Velocity-Verlet-Zeitschritt implementieren
- [ ] Test mit einem einfachen analytisch lösbaren System (z. B. harmonischer Oszillator)
- [ ] Überprüfung der Energieerhaltung
- [ ] Ausgabe der Trajektorie (z. B. im XYZ-Format zur Visualisierung)

### 2. Potenziale
- [ ] Gemeinsame Schnittstelle für Potenziale (Energie- und Kraftberechnung)
- [ ] Harmonisches Potenzial (Federn/Bindungen)
- [ ] Lennard-Jones-Potenzial
- [ ] Cutoff-Radius für Wechselwirkungen
- [ ] Optional: Coulomb-Wechselwirkung

### 3. Systemdefinition
- [ ] Simulationsbox mit periodischen Randbedingungen
- [ ] Minimum-Image-Konvention
- [ ] Initialisierung von Teilchenpositionen (z. B. Gitter) und Geschwindigkeiten (Maxwell-Boltzmann-Verteilung)
- [ ] Berechnung von Observablen: kinetische/potenzielle Energie, Temperatur

### 4. Problemdefinition über Config-Dateien
- [ ] Einlesen von Simulationsparametern (Zeitschritt, Anzahl Schritte, Box, Potenziale) aus einer Config-Datei (z. B. JSON, TOML oder YAML)
- [ ] Einlesen von Startkonfigurationen aus Dateien
- [ ] Konfigurierbare Ausgabe (Intervall, Dateiformat)

### Mögliche Erweiterungen
- [ ] Nachbarlisten (Verlet-Listen, Zellenlisten) für bessere Performance
- [ ] Thermostate (z. B. Berendsen, Langevin) für NVT-Simulationen
- [ ] Unit Tests (z. B. mit GoogleTest oder Catch2)
- [ ] Parallelisierung (z. B. OpenMP)

## Nutzung von KI-Tools

Da das Ziel dieses Projekts das Erlernen von C++ ist, ist der Code **selbst geschrieben**.

KI-Tools wie **Claude** und **GitHub Copilot** werden ausschließlich als Lernhilfen eingesetzt, und zwar:

- zum Erlernen einer sinnvollen C++-Projektstruktur (z. B. CMake, Aufteilung in Dateien)
- zur Planung des Projekts und der Meilensteine
- zum Erklären von Konzepten, Begriffen und Fehlermeldungen
