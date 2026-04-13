# Einführung in Git

## Befehle

Befehle in Reihenfolge. Plattformspezifische Befehle sind entsprechend markiert.

### Setup

1. Git installieren _(nur Windows)_
   ```
   winget install --id Git.Git -e --source winget
   ```
2. Notepad als Standard-Editor setzen _(nur Windows)_
   ```
   git config --global core.editor notepad
   ```
3. Git-Konfiguration bearbeiten (Name, E-Mail etc.)
   ```
   git config --global --edit
   ```
4. SSH-Key generieren
   ```
   ssh-keygen -t ed25519 -C "a_skywalker@edu.fhdw.de"
   ```
5. Öffentlichen SSH-Key ausgeben und in GitHub einfügen → [github.com/settings/ssh/new](https://github.com/settings/ssh/new)
   - macOS/Linux:
     ```
     cat ~/.ssh/id_ed25519.pub
     ```
   - Windows:
     ```
     cat C:\Users\<benutzername>\.ssh\id_ed25519.pub
     ```

---

### Erstes Repository

6. In einen Ordner navigieren und neues Repository anlegen
   ```
   cd Desktop && mkdir Beispiel && cd Beispiel
   git init
   ```
7. Datei erstellen
   ```
   echo "Ich bin [Name]" > name.txt
   ```
8. Datei zur Staging Area hinzufügen
   ```
   git add name.txt
   ```
9. Ersten Commit erstellen
   ```
   git commit -m "init: first commit"
   ```
