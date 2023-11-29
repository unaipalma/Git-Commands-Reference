# Referencia de Comandos Git

## Comandos Básicos

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                 | Inicia un nuevo repositorio Git.                      | `git init`                                           |
| `git clone URL`                            | Clona un repositorio existente.                       | `git clone https://github.com/ejemplo/proyecto.git`   |
| `git add nombre_archivo`                   | Añade cambios al área de preparación (staging).       | `git add archivo.txt`                                |
| `git commit -m "Mensaje de commit"`        | Guarda los cambios en el repositorio.                 | `git commit -m "Añadir nueva característica"`        |
| `git status`                               | Muestra el estado de los archivos.                    | `git status`                                         |
| `git log`                                  | Muestra el historial de commits.                      | `git log`                                            |
| `git diff`                                 | Muestra las diferencias entre los cambios.            | `git diff`                                           |

## Comandos de Ramas

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch nombre_rama`                   | Crea una nueva rama.                                 | `git branch nueva_rama`                              |
| `git checkout nombre_rama`                 | Cambia a una rama específica.                        | `git checkout nombre_rama`                           |
| `git checkout -b nombre_rama`              | Crea y cambia a una nueva rama.                      | `git checkout -b nueva_rama`                         |
| `git merge nombre_rama`                    | Fusiona cambios de otra rama a la rama actual.       | `git merge otra_rama`                                |
| `git branch -d nombre_rama`                | Elimina una rama local.                              | `git branch -d rama_a_eliminar`                     |

## Comandos Remotos

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add nombre_remoto URL`         | Conecta un repositorio local a un remoto.             | `git remote add origin https://github.com/ejemplo/proyecto.git` |
| `git push nombre_remoto nombre_rama`       | Sube cambios a una rama en un remoto.                | `git push origin master`                             |
| `git pull nombre_remoto nombre_rama`       | Descarga y fusiona cambios de un remoto.              | `git pull origin master`                             |

## Comandos de Configuración

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <sección>.<variable> valor`    | Configura opciones específicas de sistema, usuario o repositorio.| `git config user.name "Tu Nombre"`               |
| `git config --list`                        | Obtiene información de configuración.                  | `git config --list`                                  |

## Comandos Avanzados

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                | Almacena temporalmente los cambios no comprometidos.  | `git stash`                                          |
| `git stash save "Mensaje"`                 | Almacena cambios con un mensaje descriptivo.          | `git stash save "Cambios temporales para nueva funcionalidad"` |
| `git stash list`                           | Lista todas las entradas almacenadas en el stash.      | `git stash list`                                     |
| `git stash pop`                            | Aplica y elimina la última entrada en el stash.        | `git stash pop`                                      |
| `git reset --hard HEAD`                    | Desecha cambios locales y mueve HEAD al último commit.| `git reset --hard HEAD`                              |

## Comandos Adicionales

| Comando                                    | Descripción                                           | Ejemplo                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                           | Lista todas las ramas locales y remotas.                   | `git branch -a`                                      |
| `git branch -m old_branch new_branch`       | Cambia el nombre de una rama local.                               | `git branch -m old_branch new_branch`                 |
| `git push origin :old_branch`              | Elimina una rama remota.                              | `git push origin :old_branch`                         |
| `git log --oneline --graph --all`          | Muestra un historial gráfico de todos los commits.             | `git log --oneline --graph --all`                    |
| `git diff file`                           | Muestra las diferencias entre el archivo actual y el último commit. | `git diff file.txt`                                |
| `git blame file`                          | Muestra quién modificó cada línea de un archivo.          | `git blame file.txt`                                |
| `git revert commit`                       | Crea un nuevo commit que deshace los cambios de un commit anterior. | `git revert commit_hash`                          |
| `git reset commit`                        | Deshace los commits y mueve la rama hacia atrás, eliminando los cambios. | `git reset commit_hash`                            |
| `git cherry-pick commit`                  | Aplica los cambios de un commit a la rama actual.            | `git cherry-pick commit_hash`                       |
| `git submodule add repo_url`              | Agrega un submódulo al repositorio.                   | `git submodule add https://github.com/ejemplo/modulo.git` |
| `git submodule init`                      | Inicializa los submódulos después de clonar un repositorio.   | `git submodule init`                                |
| `git submodule update`                    | Actualiza los submódulos después de clonar un repositorio.       | `git submodule update`                              |
