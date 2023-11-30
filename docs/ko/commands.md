# Git 명령어 참조

## 기본 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git init`                                  | 새로운 Git 저장소를 초기화합니다.                      | `git init`                                           |
| `git clone URL`                             | 기존 저장소를 복제합니다.                             | `git clone https://github.com/example/project.git`   |
| `git add 파일명`                            | 변경 사항을 스테이징 영역에 추가합니다.               | `git add file.txt`                                   |
| `git commit -m "커밋 메시지"`              | 변경 사항을 저장소에 저장합니다.                      | `git commit -m "새로운 기능 추가"`                  |
| `git status`                                | 파일의 상태를 표시합니다.                             | `git status`                                         |
| `git log`                                   | 커밋 이력을 표시합니다.                               | `git log`                                            |
| `git diff`                                  | 변경 사항 간의 차이를 표시합니다.                    | `git diff`                                           |

## 브랜치 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch 브랜치명`                      | 새로운 브랜치를 생성합니다.                          | `git branch new_branch`                              |
| `git checkout 브랜치명`                    | 특정 브랜치로 전환합니다.                            | `git checkout branch_name`                           |
| `git checkout -b 브랜치명`                 | 새로운 브랜치를 생성하고 전환합니다.                | `git checkout -b new_branch`                         |
| `git merge 브랜치명`                       | 다른 브랜치에서 변경 사항을 현재 브랜치로 병합합니다. | `git merge other_branch`                             |
| `git branch -d 브랜치명`                   | 로컬 브랜치를 삭제합니다.                            | `git branch -d branch_to_delete`                     |

## 원격 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git remote add 원격명 URL`                 | 로컬 저장소를 원격에 연결합니다.                    | `git remote add origin https://github.com/example/project.git` |
| `git push 원격명 브랜치명`                | 변경 사항을 원격 브랜치에 푸시합니다.               | `git push origin master`                             |
| `git pull 원격명 브랜치명`                | 원격 브랜치에서 변경 사항을 가져와 병합합니다.       | `git pull origin master`                             |

## 설정 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git config <섹션>.<변수> 값`               | 시스템, 사용자 또는 저장소 설정을 구성합니다.        | `git config user.name "당신의 이름"`                |
| `git config --list`                         | 구성 정보를 가져옵니다.                               | `git config --list`                                  |

## 고급 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git stash`                                | 일시적으로 커밋되지 않은 변경 사항을 저장합니다.      | `git stash`                                         |
| `git stash save "메시지"`                  | 설명적인 메시지와 함께 변경 사항을 저장합니다.       | `git stash save "새로운 기능을 위한 임시 변경 사항"` |
| `git stash list`                           | 스태시에 저장된 모든 항목을 나열합니다.               | `git stash list`                                    |
| `git stash pop`                            | 최신 스태시 항목을 적용하고 제거합니다.              | `git stash pop`                                     |
| `git reset --hard HEAD`                    | 로컬 변경 사항을 삭제하고 HEAD를 마지막 커밋으로 이동합니다.| `git reset --hard HEAD`                             |

## 추가 명령어

| 명령어                                      | 설명                                                  | 예제                                                 |
|---------------------------------------------|-------------------------------------------------------|------------------------------------------------------|
| `git branch -a`                             | 모든 로컬 및 원격 브랜치를 나열합니다.               | `git branch -a`                                     |
| `git branch -m 이전브랜치 새로운브랜치`     | 로컬 브랜치의 이름을 변경합니다.                     | `git branch -m old_branch new_branch`                |
| `git push origin :이전브랜치`               | 원격 브랜치를 삭제합니다.                            | `git push origin :old_branch`                        |
| `git log --oneline --graph --all`          | 모든 커밋의 그래픽 히스토리를 표시합니다.           | `git log --oneline --graph --all`                   |
| `git diff 파일`                           | 현재 파일과 마지막 커밋 간의 차이를 표시합니다.    | `git diff file.txt`                                 |
| `git blame 파일`                          | 각 행을 수정한 사람을 표시합니다.                    | `git blame file.txt`                                |
| `git revert 커밋`                        | 이전 커밋의 변경 사항을 취소하는 새로운 커밋을 만듭니다.| `git revert commit_hash`                           |
| `git reset 커밋`                         | 커밋을 취소하고 브랜치를 이전 위치로 이동합니다.   | `git reset commit_hash`                             |
| `git cherry-pick 커밋`                   | 커밋에서 변경 사항을 현재 브랜치에 적용합니다.     | `git cherry-pick commit_hash`                       |
| `git submodule add 저장소 URL`           | 저장소에 서브모듈을 추가합니다.                      | `git submodule add https://github.com/example/module.git` |
| `git submodule init`                      | 저장소를 복제한 후 서브모듈을 초기화합니다.          | `git submodule init`                                |
| `git submodule update`                    | 저장소를 복제한 후 서브모듈을 업데이트합니다.      | `git submodule update`                              |
