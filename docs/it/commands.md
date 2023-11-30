# Riferimento Comandi Git

## Comandi Base

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                  | Inizializza un nuovo repository Git.                   | `git init`                                           |
| `git clone URL`                             | Clona un repository esistente.                         | `git clone https://github.com/esempio/progetto.git`   |
| `git add nome_file`                         | Aggiunge le modifiche all'area di staging.             | `git add file.txt`                                   |
| `git commit -m "Messaggio del commit"`      | Salva le modifiche nel repository.                    | `git commit -m "Aggiunto nuovo feature"`             |
| `git status`                                | Mostra lo stato dei file.                              | `git status`                                         |
| `git log`                                   | Visualizza la cronologia dei commit.                   | `git log`                                            |
| `git diff`                                  | Mostra le differenze tra le modifiche.                | `git diff`                                           |

## Comandi di Branch

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch nome_branch`                    | Crea un nuovo branch.                                 | `git branch nuovo_branch`                            |
| `git checkout nome_branch`                  | Passa a un branch specifico.                          | `git checkout nome_branch`                           |
| `git checkout -b nome_branch`               | Crea e passa a un nuovo branch.                       | `git checkout -b nuovo_branch`                       |
| `git merge nome_branch`                     | Unisce le modifiche da un altro branch nel branch corrente.| `git merge altro_branch`                             |
| `git branch -d nome_branch`                 | Cancella un branch locale.                            | `git branch -d branch_da_cancellare`                 |

## Comandi Remoti

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add nome_remoto URL`            | Collega un repository locale a un remoto.              | `git remote add origin https://github.com/esempio/progetto.git` |
| `git push nome_remoto nome_branch`          | Invia le modifiche a un branch su un remoto.          | `git push origin master`                             |
| `git pull nome_remoto nome_branch`          | Prende e unisce le modifiche da un branch remoto.     | `git pull origin master`                             |

## Comandi di Configurazione

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <sezione>.<variabile> valore`   | Configura le impostazioni di sistema, utente o repository.| `git config user.name "Tuo Nome"`                    |
| `git config --list`                         | Ottiene informazioni di configurazione.               | `git config --list`                                  |

## Comandi Avanzati

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                 | Salva temporaneamente le modifiche non ancora commesse.| `git stash`                                         |
| `git stash save "Messaggio"`                | Salva le modifiche con un messaggio descrittivo.      | `git stash save "Modifiche temporanee per nuova feature"` |
| `git stash list`                            | Elenca tutte le voci salvate in stash.                | `git stash list`                                    |
| `git stash pop`                             | Applica e rimuove l'ultima voce in stash.             | `git stash pop`                                     |
| `git reset --hard HEAD`                     | Elimina le modifiche locali e sposta HEAD all'ultimo commit.| `git reset --hard HEAD`                             |

## Comandi Aggiuntivi

| Comando                                     | Descrizione                                           | Esempio                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                             | Elenca tutti i branch locali e remoti.                | `git branch -a`                                     |
| `git branch -m vecchio_branch nuovo_branch` | Rinomina un branch locale.                            | `git branch -m vecchio_branch nuovo_branch`          |
| `git push origin :vecchio_branch`           | Elimina un branch remoto.                             | `git push origin :vecchio_branch`                    |
| `git log --oneline --graph --all`           | Mostra una storia grafica di tutti i commit.          | `git log --oneline --graph --all`                   |
| `git diff file`                            | Mostra le differenze tra il file attuale e l'ultimo commit.| `git diff file.txt`                               |
| `git blame file`                           | Visualizza chi ha modificato ogni riga di un file.    | `git blame file.txt`                                |
| `git revert commit`                        | Crea un nuovo commit che annulla le modifiche di un commit precedente.| `git revert hash_del_commit`                      |
| `git reset commit`                         | Annulla i commit e sposta il branch indietro, eliminando le modifiche.| `git reset hash_del_commit`                        |
| `git cherry-pick commit`                   | Applica le modifiche di un commit nel branch corrente.| `git cherry-pick hash_del_commit`                  |
| `git submodule add url_repo`               | Aggiunge un sotto modulo al repository.               | `git submodule add https://github.com/esempio/modulo.git` |
| `git submodule init`                       | Inizializza i sotto moduli dopo il clone di un repository.| `git submodule init`                               |
| `git submodule update`                     | Aggiorna i sotto moduli dopo il clone di un repository.| `git submodule update`                             |
