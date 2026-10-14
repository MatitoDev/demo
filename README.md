# Demo

## Git-Workflow

Ein typischer Ablauf: Repository bereitstellen, auf einem Branch arbeiten, Änderungen prüfen und committen, anschließend mit dem Remote-Repository synchronisieren.

### 1. Repository bereitstellen

Ein vorhandenes Repository klonen:

```bash
git clone <repository-url>
cd <repository-ordner>
```

Oder ein neues Repository im aktuellen Ordner anlegen:

```bash
git init
```

Remote-Verbindungen anzeigen:

```bash
git remote -v
```

### 2. Arbeitsstand aktualisieren und Branch vorbereiten

Vor der Arbeit den aktuellen Stand vom Remote holen:

```bash
git pull
```

Branches anzeigen:

```bash
git branch
```

Neuen Branch erstellen und direkt wechseln:

```bash
git checkout -b <branch-name>
```

Zu einem vorhandenen Branch wechseln:

```bash
git checkout <branch-name>
```

### 3. Änderungen prüfen und vorbereiten

Arbeitsstand anzeigen:

```bash
git status
```

Änderungen im Detail ansehen:

```bash
git diff
```

Dateien für den nächsten Commit vormerken:

```bash
git add <dateiname>
git add .
```

Eine Datei wieder aus der Vormerkung nehmen:

```bash
git restore --staged <dateiname>
```

Nicht gespeicherte Änderungen an einer Datei verwerfen:

```bash
git restore <dateiname>
```

### 4. Änderungen committen

Vorgemerkte Änderungen als Commit speichern:

```bash
git commit -m "Beschreibung der Änderung"
```

Commit-Verlauf anzeigen:

```bash
git log
```

### 5. Änderungen teilen und Branches zusammenführen

Eigene Commits zum Remote-Repository senden:

```bash
git push
```

Um einen Branch in einen anderen zu übernehmen, zuerst zum Ziel-Branch wechseln und dann den Arbeits-Branch mergen:

```bash
git checkout <ziel-branch>
git pull
git merge <arbeits-branch>
git push
```

### Hilfe

Hilfe zu einem Git-Befehl anzeigen:

```bash
git help <befehl>
```
