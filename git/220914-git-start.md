# Today I Learned

## 13:00~14:00
- Git의 설치와 기본명령어(pwd/cd/ls/mkdir etc)
- touch 명령어로 생성하는 파일은 텍스트 기반 파일only
- remove는 접근하는 방법을 지우는 것

## 14:00~15:00
### Vim 코드
- Normal mode(press esc on anymode)
- Insert mode(press i on normal mode)
- Command mode(press : on normal mode)
- Visual mode(press v on normal mode)
- vim내에서의 구두점 사용


## 15:00~16:00
- github account sign up
- Create new repo on git hub/clone on git-bash
- clone > git clone (url)

## 16:00~17:00
### git의 진행과정과 명령어
- add > commit > push(origin main)
- 여타 명령어 git (config --list/status/add/commit/push)
- vi를 이용한 파일의 수정 후add와 commit을 이용하여 remote server에 반영
- personal token의 생성

## 17:00~18:00
### git의 conventional rule
- prefix(feat/fix/docs/test/conf)

### .gitignore
- create후 vi를 통해 무시할 특징을 정함
- gitignore.io를 통해 간편하게 설정 가능

## 19:00~20:00
- TIL
- Directory의 생성은 commit의 필요가 없음
- > directory는 경로의 생성이기 떄문
- new command : git status -uall

## 20:00~22:00
### Branch
- git branch ->조회
- main > default
- commit이 시간의 개념이라면 branch는 공간의 개념 > 잘 이해는 안감
- git switch {} 이동
- checkout > restore/switch로 나뉨 기능이
- git branch -D {branch_name}
- merge > 밀어내는 게 아닌 당기는 것(git merge {적용시킬 branch})

### merge conflict
- main/branch에서 같은 지점에서 일어난 변경은
- merge시에 충돌이 일어남,
- 이때 일어난 충돌을 vi를 통해서 수정해야함(특수문자도 당연히 삭제)
