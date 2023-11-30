# Referência de Comandos Git

## Comandos Básicos

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                  | Inicializa um novo repositório Git.                   | `git init`                                           |
| `git clone URL`                             | Clona um repositório existente.                       | `git clone https://github.com/exemplo/projeto.git`    |
| `git add nome_do_arquivo`                   | Adiciona alterações à área de preparação.              | `git add arquivo.txt`                                |
| `git commit -m "Mensagem do commit"`        | Salva alterações no repositório.                      | `git commit -m "Adicionar novo recurso"`             |
| `git status`                                | Mostra o status dos arquivos.                         | `git status`                                         |
| `git log`                                   | Exibe o histórico de commits.                         | `git log`                                            |
| `git diff`                                  | Mostra as diferenças entre as alterações.             | `git diff`                                           |

## Comandos de Branch

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch nome_do_branch`                 | Cria um novo branch.                                  | `git branch novo_branch`                             |
| `git checkout nome_do_branch`               | Muda para um branch específico.                       | `git checkout nome_do_branch`                        |
| `git checkout -b nome_do_branch`            | Cria e muda para um novo branch.                      | `git checkout -b novo_branch`                        |
| `git merge nome_do_branch`                  | Mescla alterações de outro branch no branch atual.    | `git merge outro_branch`                             |
| `git branch -d nome_do_branch`              | Exclui um branch local.                               | `git branch -d branch_a_excluir`                     |

## Comandos Remotos

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add nome_remoto URL`            | Conecta um repositório local a um remoto.             | `git remote add origin https://github.com/exemplo/projeto.git` |
| `git push nome_remoto nome_branch`          | Envia alterações para um branch em um repositório remoto.| `git push origin master`                             |
| `git pull nome_remoto nome_branch`          | Obtém e mescla alterações de um branch remoto.        | `git pull origin master`                             |

## Comandos de Configuração

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <seção>.<variável> valor`       | Configurações do sistema, usuário ou repositório.     | `git config user.name "Seu Nome"`                   |
| `git config --list`                         | Obtém informações de configuração.                    | `git config --list`                                  |

## Comandos Avançados

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                 | Armazena temporariamente alterações não comprometidas.| `git stash`                                         |
| `git stash save "Mensagem"`                 | Salva alterações com uma mensagem descritiva.         | `git stash save "Alterações temporárias para novo recurso"` |
| `git stash list`                            | Lista todas as entradas armazenadas no stash.         | `git stash list`                                    |
| `git stash pop`                             | Aplica e remove a última entrada do stash.            | `git stash pop`                                     |
| `git reset --hard HEAD`                     | Descarta alterações locais e move HEAD para o último commit.| `git reset --hard HEAD`                             |

## Comandos Adicionais

| Comando                                     | Descrição                                             | Exemplo                                              |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                             | Lista todos os branches locais e remotos.             | `git branch -a`                                     |
| `git branch -m antigo_branch novo_branch`   | Renomeia um branch local.                             | `git branch -m antigo_branch novo_branch`            |
| `git push origin :antigo_branch`            | Exclui um branch remoto.                              | `git push origin :antigo_branch`                     |
| `git log --oneline --graph --all`           | Mostra um histórico gráfico de todos os commits.      | `git log --oneline --graph --all`                   |
| `git diff arquivo`                          | Mostra as diferenças entre o arquivo atual e o último commit.| `git diff arquivo.txt`                             |
| `git blame arquivo`                         | Exibe quem modificou cada linha de um arquivo.        | `git blame arquivo.txt`                             |
| `git revert commit`                         | Cria um novo commit que desfaz as alterações de um commit anterior.| `git revert hash_do_commit`                        |
| `git reset commit`                          | Desfaz commits e move o branch de volta, descartando alterações.| `git reset hash_do_commit`                         |
| `git cherry-pick commit`                    | Aplica alterações de um commit no branch atual.       | `git cherry-pick hash_do_commit`                   |
| `git submodule add url_repo`                | Adiciona um submódulo ao repositório.                 | `git submodule add https://github.com/exemplo/modulo.git` |
| `git submodule init`                        | Inicializa submódulos após o clone de um repositório. | `git submodule init`                               |
| `git submodule update`                      | Atualiza submódulos após o clone de um repositório.   | `git submodule update`                             |
