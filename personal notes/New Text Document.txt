#### Schritt-für-Schritt-Anleitung zum Erstellen eines lokalen Repositorys (in VS Code):

- Verwende VS Code, um die Änderungen visuell zu sehen.
- Stelle sicher, dass du dich in VS Code bei GitHub anmeldest.
- Befolge diese Schritte:

1. Öffne dein gewünschtes Verzeichnis in VS Code (`es sollte mindestens eine Markdown-Datei enthalten`. Dies liegt daran, dass Git keine leeren Verzeichnisse verfolgt).
2. Öffne das Terminal in VS Code (`Strg + J`)
3. Initialisiere ein neues Git-Repository **`(tue dies nur einmal pro Projekt)`**:
   ```bash
   git init
   ```
   - Dies erstellt einen `.git`-Ordner in deinem Projektverzeichnis.
   - Du wirst sehen, dass alle Dateien jetzt grün mit einem U-Symbol (untracked/unverfolgt) im Source Control-Tab sind.
   - Das bedeutet, dass Git diese Dateien verfolgt, sie aber noch nicht für den Commit gestaged sind.
4. Stage die Dateien für den Commit:
   ```bash
   git add .
   ```
   - Der `.` nach `git add` bedeutet `BITTE ALLE DATEIEN HINZUFÜGEN` im aktuellen Verzeichnis.
   - Die `U`-Symbole ändern sich zu `A` (added/hinzugefügt) im Source Control-Tab.
   - Optional kannst du bestimmte Dateien stagen, indem du `.` durch den Dateinamen ersetzt. Wenn du zum Beispiel nur `README.md` stagen möchtest, würdest du ausführen:
     ```bash
     git add README.md
     ```
5. Committe die gestageten Dateien mit einer Nachricht:
   ```bash
   git commit -m "Initial commit"
   ```
   - Das `-m`-Flag ermöglicht es dir, eine Commit-Nachricht zu deinen Änderungen hinzuzufügen.
6. An diesem Punkt verwenden wir den `Source Control`-Tab in VS Code, um eine Verbindung zu einem Remote-Repository auf GitHub herzustellen.
   - Klicke auf den `Publish to GitHub`-Button.
   - Gib im Suchfeld den Namen deines neuen Repositorys ein (falls erforderlich).
   - Wähle die Sichtbarkeit deines Repositorys (öffentlich oder privat).
   - Klicke auf `Publish Repository`.
   - VS Code fügt automatisch die Remote-URL hinzu und pusht deine Änderungen.
7. Überprüfe, ob deine Änderungen nach GitHub gepusht wurden, indem du dein Repository auf der GitHub-Website besuchst.