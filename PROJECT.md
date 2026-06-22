# ProjectX – Projektübersicht

Single Source of Truth für Struktur, Gruppen und Aufgabenbereiche.

## Repository-Inhalt

| Datei | Beschreibung |
|-------|--------------|
| [`aufgaben.py`](aufgaben.py) | 100 Übungsfunktionen (Stubs mit Docstrings) |
| [`README.md`](README.md) | Anleitung für Studierende |
| [`tests/test_gruppen_zuordnung.py`](tests/test_gruppen_zuordnung.py) | Automatische Prüfung der Gruppenkommentare |

## Gruppenaufteilung (5 Gruppen, je 20 Aufgaben)

Zuordnung laut Board (oben nach unten). Jede Gruppe hat zwei Personen.

| Gruppe | GitHub-Handles | Aufgaben | Thema |
|--------|----------------|----------|-------|
| 1 | `Dni-schaf`, `smartsys` | `aufgabe_001` – `aufgabe_020` | Strings & Listen-Basics |
| 2 | `Tobbyte`, `DuclosNgassa` | `aufgabe_021` – `aufgabe_040` | Listen-Operationen & Dict-Einstieg |
| 3 | `Vincent-Pieper`, `SoerenNeumann1985` | `aufgabe_041` – `aufgabe_060` | Dicts, Sets & Mathematik |
| 4 | `LarsPetschke`, `PaddePain` | `aufgabe_061` – `aufgabe_080` | Zahlen, Skalierung & Matrizen |
| 5 | `binudio1`, `iSayaGen` | `aufgabe_081` – `aufgabe_100` | Algorithmen & Text-Parsing |

## Aufgaben pro Gruppe (Kurzüberblick)

### Gruppe 1 (001–020)

String-Manipulation, Wortlisten, Listen-Mathematik (Summe, Mittelwert, Min/Max, Sortieren).

### Gruppe 2 (021–040)

Listen sortieren/filtern, Utilities (flatten, chunk, rotate), Dict-Grundlagen.

### Gruppe 3 (041–060)

Dict-Operationen, Set-Operationen, Duplikate, Fakultät, Fibonacci, Primzahlen, GGT/KGV.

### Gruppe 4 (061–080)

Zahlenformatierung, Skalierung, gleitender Mittelwert, Dict-Vergleich, Matrizen.

### Gruppe 5 (081–100)

Suche & Sortierung, Anagramme, Tokenisierung, E-Mail/URL/KV-Parsing.

## Regeln für Studierende

- Nur den eigenen Aufgabenbereich in `aufgaben.py` bearbeiten.
- Gruppenkommentare (`# Gruppe: ...`) nicht ändern.
- Vor Abgabe: `python3 -m pytest tests/test_gruppen_zuordnung.py`
- Branch-Naming: `gruppe-<nr>/<github-handle>` (z. B. `gruppe-1/Dni-schaf`)

## Änderungshistorie

- **2026-06-22**: Neue Gruppenaufteilung nach Board (5×2 Personen, 20 Aufgaben pro Gruppe). Siehe [ADR](../.cursor/adr/0001-neue-gruppenaufteilung.md).
