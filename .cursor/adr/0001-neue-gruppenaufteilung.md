# ADR 0001: Neue Gruppenaufteilung nach Board

## Status

Angenommen (2026-06-22)

## Kontext

Das Übungsrepository `ProjectX` enthält 100 Python-Stub-Funktionen in `aufgaben.py`.
Studierende arbeiten in Gruppen an zugewiesenen Aufgabenbereichen, um Merge-Konflikte
zu vermeiden.

Die bisherige Zuordnung (Handles wie `patricznr1`, `it-student`, …) entsprach nicht
mehr der aktuellen Kursgruppe auf dem Board. Eine neue Aufteilung mit fünf Gruppen
à zwei Personen war erforderlich.

## Entscheidung

1. **Gruppen-Handles** werden an das Board angepasst (von oben nach unten):

   | Gruppe | Handles |
   |--------|---------|
   | 1 | `Dni-schaf`, `smartsys` |
   | 2 | `Tobbyte`, `DuclosNgassa` |
   | 3 | `Vincent-Pieper`, `SoerenNeumann1985` |
   | 4 | `LarsPetschke`, `PaddePain` |
   | 5 | `binudio1`, `iSayaGen` |

2. **Aufgabenblöcke bleiben 20er-Segmente** (001–020, 021–040, …, 081–100).
   Die thematische Progression (Strings → Listen → Dicts/Sets → Matrizen → Algorithmen)
   bleibt unverändert.

3. **Nur Kommentare und Dokumentation** werden geändert; Funktionsnamen, Signaturen
   und Docstrings bleiben gleich.

4. **`PROJECT.md`** wird als Single Source of Truth für Gruppen und Aufgabenbereiche
   eingeführt.

5. **`tests/test_gruppen_zuordnung.py`** prüft die Zuordnung automatisch (TDD).

## Begründung

- Gleichmäßige Arbeitslast: je 20 Aufgaben pro Gruppe.
- Einheitliche Gruppengröße: 2 Personen (vorher hatte Gruppe 5 drei Personen).
- Bestehende Lernkurve der Aufgaben bleibt erhalten → kein Risiko durch Umstrukturierung.
- Automatisierter Test verhindert Drift zwischen `aufgaben.py` und Dokumentation.

## Konsequenzen

### Positiv

- README, `PROJECT.md` und `aufgaben.py` sind synchron.
- Studierende können die Zuordnung lokal verifizieren.

### Negativ / Migration

- Studierende mit alten Branches müssen neue Branches nach aktueller Aufteilung anlegen.
- Bereits implementierte Aufgaben in alten Bereichen passen ggf. nicht mehr zur neuen Gruppe.

## Alternativen (verworfen)

- **Neuverteilung der Aufgabeninhalte**: Abgelehnt, da unnötiger Aufwand und Bruch der Lernkurve.
- **4 Gruppen à 25 Aufgaben**: Abgelehnt; Board zeigt explizit 5 Gruppen.
