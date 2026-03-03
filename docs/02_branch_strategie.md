# Branching-Strategie

## Verwendete Strategie

Für dieses Repository wird eine einfache Feature-Branch-Strategie verwendet.

Der Hauptbranch `main` enthält immer eine stabile Version des Projekts.  
Neue Änderungen werden niemals direkt auf `main` gemacht.

Stattdessen wird für jede neue Aufgabe oder Funktion ein eigener Branch erstellt.

Beispiel:

- `feat/Strategie`
- `feat/Automatisierung`
- `fix/cleanup`

## Workflow

Der typische Ablauf ist:

1. Von `main` einen neuen Feature-Branch erstellen.
2. Änderungen im Feature-Branch durchführen.
3. Änderungen committen und zum Remote-Repository pushen.
4. Einen Pull Request erstellen.
5. Der Pull Request wird überprüft und danach in `main` gemerged.

## Vorteile dieser Strategie

Diese Strategie hat mehrere Vorteile:

- Der `main` Branch bleibt immer stabil.
- Änderungen können isoliert entwickelt werden.
- Pull Requests ermöglichen Code-Review.
- Konflikte werden früh erkannt.

## Branch-Schutz

Der Branch `main` wird zusätzlich durch Branch Protection Rules geschützt.

Das bedeutet:

- Änderungen dürfen nicht direkt auf `main` gepusht werden.
- Änderungen müssen über Pull Requests erfolgen.