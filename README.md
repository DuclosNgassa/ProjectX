# Python-Übungsset (100 Funktionen)

Dieses Repository enthält 100 Basis-Übungsfunktionen in `aufgaben.py`. Jede
Funktion hat einen deutschen Docstring, `pass` als Platzhalter und soll von den
Studierenden implementiert werden. Fokus: Strings, Listen, Dicts/Sets,
Schleifen, einfache Mathematik und saubere Funktionalität.

## Gruppenaufteilung (4 Gruppen laut Board)

Die aktuelle Referenz für Gruppen und Aufgabenbereiche ist [`PROJECT.md`](PROJECT.md).

- **Gruppe 1** (Dennis `dbudb`, Linda `lindaEbbert`): Funktionen 1–25 (`aufgabe_001` bis `aufgabe_025`)
- **Gruppe 2** (Martin `Harangason`, Thorsten `ThorKel1202`): Funktionen 26–50 (`aufgabe_026` bis `aufgabe_050`)
- **Gruppe 3** (Marcel `maro-101`, Hans-Günter `HGKlemp`): Funktionen 51–75 (`aufgabe_051` bis `aufgabe_075`)
- **Gruppe 4** (Aylin `Aylin65`, Jugo `jugomit`): Funktionen 76–100 (`aufgabe_076` bis `aufgabe_100`)

Hinweis: Die Nummer ist im Funktionsnamen enthalten. Bitte bearbeitet nur den
euch zugewiesenen Bereich, damit Merge-Konflikte minimiert werden. Eure Namen
stehen auch direkt als Kommentar über jeder Aufgabe in `aufgaben.py`.

Wenn ihr zuvor mit einer älteren 5-Gruppen-Aufteilung (je 20 Aufgaben) gearbeitet
habt, legt neue Branches pro Aufgabe nach der aktuellen [`PROJECT.md`](PROJECT.md) an.

## Vorgehensweise für Studierende

**Branch-Schema:** `gruppe-x/github-name/aufgabe-xxx` (ein Branch pro Aufgabe)

Die Schritte 3–8 wiederholt ihr für jede Aufgabe in eurem Bereich.

1. Repository klonen: `git clone <repo-url>`
2. In das Repo wechseln: `cd ProjectX`
3. Eigenen Branch pro Aufgabe anlegen (Beispiel Gruppe 1, GitHub-Name `dbudb`,
   Aufgabe `aufgabe_001`):
  - `git checkout master` (bzw. `main`)
  - `git pull origin master` (bzw. `git pull origin main`)
  - `git checkout -b gruppe-1/dbudb/aufgabe-001`
4. Nur die jeweilige Funktion in `aufgaben.py` implementieren (Docstring lesen).
5. Änderungen prüfen: `git status`
6. Änderungen vormerken und committen:
  - `git add aufgaben.py`
  - `git commit -m "Implementiere aufgabe_001"`
7. Branch pushen: `git push origin gruppe-1/dbudb/aufgabe-001`
8. Euren Branch in `master` (oder `main`) mergen:
  - `git checkout master` (bzw. `git checkout main`)
  - `git pull origin master` (bzw. `git pull origin main`)
  - `git merge gruppe-1/dbudb/aufgabe-001`
  - Bei Konflikten: markierte Stellen lösen, dann `git add` und
    `git commit` (falls Git keinen Merge-Commit erstellt hat)
  - `git push origin master` (bzw. `git push origin main`)
9. Optional: Statt lokalem Merge einen Pull Request (PR) im Git-Host erstellen.
  Reviewer: Dozent oder Teamlead. Feedback einarbeiten und Branch/PR aktualisieren.
10. Nächste Aufgabe: ab Schritt 3 mit neuem Branch (z. B. `gruppe-1/dbudb/aufgabe-002`).

## Qualitätsleitplanken

- Halte dich an PEP 8 (Lesbarkeit vor Cleverness).
- Sinnvolle Variablennamen, kurze Funktionen, keine unnötigen globalen Zustände.
- Docstrings nicht löschen; ergänze Beispiele, falls hilfreich.
- Prüfe Randfälle (leere Listen, None, negative Zahlen, Sonderzeichen).
- Schreibe kleine, wiederverwendbare Hilfsfunktionen nur, wenn nötig.

## Konflikt vermeiden

- Arbeite ausschließlich im zugewiesenen Funktionsbereich.
- Ziehe vor neuem Work `git pull origin master` (bzw. `main`, oder `git fetch` +
  `git rebase`).
- Bei Konflikten: ruhig bleiben, Konflikt markieren, lokal prüfen, erst dann
committen.

## Abgabeformat

- Ein Branch und ein Merge pro Aufgabe in `master`/`main` (PR optional).
- Branch-Name: `gruppe-x/github-name/aufgabe-xxx` (z. B. `gruppe-1/dbudb/aufgabe-001`).
- Commit-Messages: kurz und beschreibend (z. B. `Implementiere aufgabe_001`).
- Keine Änderungen an fremden Bereichen oder an der Gruppenaufteilung.

Viel Erfolg und fragt bei Unklarheiten früh nach!
