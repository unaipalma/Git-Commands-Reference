# Référence des Commandes Git

## Commandes de Base

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                   | Initialise un nouveau dépôt Git.                      | `git init`                                           |
| `git clone URL`                              | Clone un dépôt existant.                               | `git clone https://github.com/exemple/projet.git`    |
| `git add nom_fichier`                        | Ajoute des modifications à la zone de préparation.     | `git add fichier.txt`                                |
| `git commit -m "Message de commit"`          | Enregistre les modifications dans le dépôt.           | `git commit -m "Ajouter une nouvelle fonctionnalité"`|
| `git status`                                 | Affiche l'état des fichiers.                           | `git status`                                         |
| `git log`                                    | Affiche l'historique des commits.                      | `git log`                                            |
| `git diff`                                   | Affiche les différences entre les modifications.      | `git diff`                                           |

## Commandes de Branche

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch nom_branche`                     | Crée une nouvelle branche.                            | `git branch nouvelle_branche`                        |
| `git checkout nom_branche`                   | Bascule vers une branche spécifique.                   | `git checkout nom_branche`                           |
| `git checkout -b nom_branche`                | Crée et bascule vers une nouvelle branche.            | `git checkout -b nouvelle_branche`                   |
| `git merge nom_branche`                      | Fusionne les modifications d'une autre branche dans la branche actuelle.| `git merge autre_branche`                      |
| `git branch -d nom_branche`                  | Supprime une branche locale.                           | `git branch -d branche_a_supprimer`                  |

## Commandes Distantes

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add nom_remote URL`              | Connecte un dépôt local à un dépôt distant.            | `git remote add origin https://github.com/exemple/projet.git` |
| `git push nom_remote nom_branche`           | Pousse les modifications vers une branche d'un dépôt distant.| `git push origin master`                          |
| `git pull nom_remote nom_branche`           | Récupère et fusionne les modifications d'une branche distante.| `git pull origin master`                          |

## Commandes de Configuration

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <section>.<variable> valeur`    | Configure les paramètres du système, de l'utilisateur ou du dépôt.| `git config user.name "Votre Nom"`             |
| `git config --list`                          | Obtient des informations de configuration.             | `git config --list`                                  |

## Commandes Avancées

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                  | Stocke temporairement les modifications non validées. | `git stash`                                          |
| `git stash save "Message"`                   | Stocke les modifications avec un message descriptif.   | `git stash save "Modifications temporaires pour nouvelle fonctionnalité"` |
| `git stash list`                             | Liste toutes les entrées stockées dans la stash.       | `git stash list`                                     |
| `git stash pop`                              | Applique et supprime la dernière entrée de la stash.   | `git stash pop`                                      |
| `git reset --hard HEAD`                      | Abandonne les modifications locales et déplace HEAD vers le dernier commit.| `git reset --hard HEAD`                          |

## Commandes Additionnelles

| Commande                                     | Description                                           | Exemple                                             |
|----------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                              | Liste toutes les branches locales et distantes.       | `git branch -a`                                      |
| `git branch -m ancienne_branche nouvelle_branche`| Renomme une branche locale.                          | `git branch -m ancienne_branche nouvelle_branche`     |
| `git push nom_remote :ancienne_branche`      | Supprime une branche distante.                        | `git push origin :ancienne_branche`                   |
| `git log --oneline --graph --all`            | Affiche un historique graphique de tous les commits.  | `git log --oneline --graph --all`                    |
| `git diff fichier`                           | Affiche les différences entre le fichier actuel et le dernier commit.| `git diff fichier.txt`                            |
| `git blame fichier`                          | Affiche qui a modifié chaque ligne d'un fichier.      | `git blame fichier.txt`                              |
| `git revert commit`                          | Crée un nouveau commit annulant les modifications d'un commit précédent.| `git revert hash_commit`                         |
| `git reset commit`                           | Annule les commits et déplace la branche en arrière, en abandonnant les modifications.| `git reset hash_commit`                           |
| `git cherry-pick commit`                     | Applique les modifications d'un commit à la branche actuelle.| `git cherry-pick hash_commit`                      |
| `git submodule add url_repo`                 | Ajoute un sous-module au dépôt.                      | `git submodule add https://github.com/exemple/module.git` |
| `git submodule init`                         | Initialise les sous-modules après le clonage d'un dépôt.| `git submodule init`                                |
| `git submodule update`                       | Met à jour les sous-modules après le clonage d'un dépôt.| `git submodule update`                              |
