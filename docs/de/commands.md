# Git Befehlsreferenz

## Grundlegende Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git init`                                   | Initialisiert ein neues Git-Repository.               | `git init`                                          |
| `git clone URL`                              | Klonen eines vorhandenen Repositorys.                 | `git clone https://github.com/beispiel/projekt.git` |
| `git add Dateiname`                          | Änderungen dem Zwischenspeicher hinzufügen.           | `git add datei.txt`                                 |
| `git commit -m "Commit-Nachricht"`           | Änderungen im Repository speichern.                   | `git commit -m "Neues Feature hinzufügen"`           |
| `git status`                                 | Zeigt den Status der Dateien an.                      | `git status`                                        |
| `git log`                                    | Zeigt die Commit-Historie an.                         | `git log`                                           |
| `git diff`                                   | Zeigt Unterschiede zwischen Änderungen an.            | `git diff`                                          |

## Branch-Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git branch Branchenname`                     | Erstellt einen neuen Branch.                          | `git branch neuer_branch`                           |
| `git checkout Branchenname`                   | Wechselt zu einem bestimmten Branch.                  | `git checkout branchenname`                        |
| `git checkout -b Branchenname`                | Erstellt und wechselt zu einem neuen Branch.          | `git checkout -b neuer_branch`                     |
| `git merge Branchenname`                      | Mergt Änderungen von einem anderen Branch in den aktuellen.| `git merge anderer_branch`                         |
| `git branch -d Branchenname`                  | Löscht einen lokalen Branch.                          | `git branch -d zu_loeschender_branch`               |

## Remote-Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git remote add Remote-Name URL`             | Verbindet ein lokales Repository mit einem Remote.    | `git remote add origin https://github.com/beispiel/projekt.git` |
| `git push Remote-Name Branchenname`          | Überträgt Änderungen an einen Branch in einem Remote.  | `git push origin master`                            |
| `git pull Remote-Name Branchenname`          | Holt und merged Änderungen von einem Remote-Branch.   | `git pull origin master`                            |

## Konfigurations-Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git config <Abschnitt>.<Variable> Wert`     | Konfiguriert System-, Benutzer- oder Repositoryeinstellungen.| `git config benutzer.name "Dein Name"`             |
| `git config --list`                          | Zeigt Konfigurationsinformationen an.                 | `git config --list`                                |

## Fortgeschrittene Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git stash`                                  | Speichert vorübergehend nicht committed Änderungen.   | `git stash`                                        |
| `git stash save "Nachricht"`                 | Speichert Änderungen mit einer beschreibenden Nachricht.| `git stash save "Temporäre Änderungen für neues Feature"` |
| `git stash list`                             | Zeigt alle Einträge im Stash an.                      | `git stash list`                                   |
| `git stash pop`                              | Wendet den letzten Stash-Eintrag an und entfernt ihn. | `git stash pop`                                    |
| `git reset --hard HEAD`                      | Verwirft lokale Änderungen und verschiebt HEAD zum letzten Commit.| `git reset --hard HEAD`                           |

## Zusätzliche Befehle

| Befehl                                       | Beschreibung                                          | Beispiel                                           |
|----------------------------------------------|-------------------------------------------------------|-----------------------------------------------------|
| `git branch -a`                              | Listet alle lokalen und Remote-Branches auf.          | `git branch -a`                                    |
| `git branch -m alter_branch neuer_branch`     | Benennt einen lokalen Branch um.                      | `git branch -m alter_branch neuer_branch`          |
| `git push origin :alter_branch`              | Löscht einen Remote-Branch.                           | `git push origin :alter_branch`                    |
| `git log --oneline --graph --all`            | Zeigt eine grafische Historie aller Commits an.       | `git log --oneline --graph --all`                  |
| `git diff Datei`                             | Zeigt Unterschiede zwischen der aktuellen Datei und dem letzten Commit.| `git diff datei.txt`                            |
| `git blame Datei`                            | Zeigt an, wer jede Zeile einer Datei geändert hat.    | `git blame datei.txt`                              |
| `git revert Commit`                          | Erstellt einen neuen Commit, der die Änderungen eines vorherigen Commits rückgängig macht.| `git revert commit_hash`                        |
| `git reset Commit`                           | Macht Commits rückgängig und verschiebt den Branch zurück, verwirft Änderungen.| `git reset commit_hash`                           |
| `git cherry-pick Commit`                     | Wendet Änderungen aus einem Commit auf den aktuellen Branch an.| `git cherry-pick commit_hash`                   |
| `git submodule add Repo_URL`                 | Fügt dem Repository ein Submodul hinzu.               | `git submodule add https://github.com/beispiel/modul.git` |
| `git submodule init`                         | Initialisiert Submodule nach dem Klonen eines Repositorys.| `git submodule init`                              |
| `git submodule update`                       | Aktualisiert Submodule nach dem Klonen eines Repositorys.| `git submodule update`                            |
