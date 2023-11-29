# Git Commands Reference

## Basic Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                 | Initialize a new Git repository.                      | `git init`                                           |
| `git clone URL`                            | Clone an existing repository.                         | `git clone https://github.com/example/project.git`   |
| `git add file_name`                        | Add changes to the staging area.                      | `git add file.txt`                                   |
| `git commit -m "Commit message"`           | Save changes to the repository.                       | `git commit -m "Add new feature"`                    |
| `git status`                               | Show the status of files.                             | `git status`                                         |
| `git log`                                  | Display commit history.                               | `git log`                                            |
| `git diff`                                 | Show differences between changes.                     | `git diff`                                           |

## Branch Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch branch_name`                   | Create a new branch.                                 | `git branch new_branch`                              |
| `git checkout branch_name`                 | Switch to a specific branch.                          | `git checkout branch_name`                           |
| `git checkout -b branch_name`              | Create and switch to a new branch.                   | `git checkout -b new_branch`                         |
| `git merge branch_name`                    | Merge changes from another branch into the current one.| `git merge other_branch`                             |
| `git branch -d branch_name`                | Delete a local branch.                               | `git branch -d branch_to_delete`                     |

## Remote Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add remote_name URL`           | Connect a local repository to a remote.              | `git remote add origin https://github.com/example/project.git` |
| `git push remote_name branch_name`         | Push changes to a branch on a remote.                | `git push origin master`                             |
| `git pull remote_name branch_name`         | Fetch and merge changes from a remote branch.        | `git pull origin master`                             |

## Configuration Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <section>.<variable> value`    | Configure system, user, or repository settings.      | `git config user.name "Your Name"`                  |
| `git config --list`                        | Get configuration information.                       | `git config --list`                                  |

## Advanced Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                | Temporarily store uncommitted changes.               | `git stash`                                          |
| `git stash save "Message"`                 | Save changes with a descriptive message.             | `git stash save "Temporary changes for new feature"` |
| `git stash list`                           | List all entries stored in the stash.                | `git stash list`                                     |
| `git stash pop`                            | Apply and remove the latest stash entry.             | `git stash pop`                                      |
| `git reset --hard HEAD`                    | Discard local changes and move HEAD to the last commit.| `git reset --hard HEAD`                              |

## Additional Commands

| Command                                    | Description                                           | Example                                              |
|--------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                           | List all local and remote branches.                   | `git branch -a`                                      |
| `git branch -m old_branch new_branch`       | Rename a local branch.                               | `git branch -m old_branch new_branch`                 |
| `git push origin :old_branch`              | Delete a remote branch.                              | `git push origin :old_branch`                         |
| `git log --oneline --graph --all`          | Show a graphical history of all commits.             | `git log --oneline --graph --all`                    |
| `git diff file`                           | Show differences between the current file and the last commit.| `git diff file.txt`                                |
| `git blame file`                          | Display who modified each line of a file.           | `git blame file.txt`                                |
| `git revert commit`                       | Create a new commit that undoes the changes of a previous commit.| `git revert commit_hash`                          |
| `git reset commit`                        | Undo commits and move the branch back, discarding changes.| `git reset commit_hash`                            |
| `git cherry-pick commit`                  | Apply changes from a commit to the current branch.  | `git cherry-pick commit_hash`                       |
| `git submodule add repo_url`              | Add a submodule to the repository.                   | `git submodule add https://github.com/example/module.git` |
| `git submodule init`                      | Initialize submodules after cloning a repository.   | `git submodule init`                                |
| `git submodule update`                    | Update submodules after cloning a repository.       | `git submodule update`                              |
