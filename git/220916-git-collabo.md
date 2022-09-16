# Today I Learned

## 13:00 ~ 14:00
- 지금까지의 과정이 정방향이라면 이번에는 역방향 내용임

### Git에서의 rename
- 일반적으로 mv 커맨드는 git에서 오류
>  이는 과정이 삭제 후 재생성이기 때문
- 따라서 사용하는 커맨드 = git mv {original_name} {new_name}

### Git에서의 Undoing
- git add 이전, 즉 stage에 올라가기 전 시점
- git restore {file}
> 이를 통해 현 작업 directory 하 모든 변화량을 최신 commit으로 되돌림


### Unstaging
- git add를 통한 staging이 완료된 파일의 unstage의 커맨드는 다음과 같음
> git reset HEAD {file}


### Reverting
- 일반적인 경우 reset은 대단히 위험한 선택
- 따라서 Commit의 revert는  log에 남긴해도 git revert 기능을 사용해야 함
> git revert --no-commit HEAD~3..
- 이는 HEAD에서 3번째 줄까지 순차적으로 되돌림을 의미
- 이 떄 git lg를 통해 로그를 확인하면 commit기록이 남아있음


## 14:00 ~ 18:00

### COllaboration with teammate using github
(1) 팀장 : Organization을 만든다
(2) Issue Template을 생성
(3) Clone 후 git flow init 커맨드 실행
(4) 대상 파일 생성 후 origin develop으로 push
(5) 팀원 : develop 확인 후 fork
(6) 나의 repo 방문 전 내 할 일 issue 등록
(7) fork한 repo clone, git flow init
(8) git flow feature start {file}
> -----WORK------
(9) git flow feature finish {file}
(10) push to origin develop
(11) Open Pull Request
(12) 팀장 : code review 후 Approve/Comment/Change request
(13) 팀원 : 추가 작업 후 origin develop으로 push
(14) merge conflict가 있다면 조직의 develop local로 pull하여 conflict 해결 후 add, commit, push
(15) 팀장 : Merge pull request


여기까지 마무리 되었으면 Release process에 들어감
- git flow release start/finish v1.0
- 이후 팀장 Local repo에서 Remote repo에 Main/Develop Branch로 push해줘야 함
- ++ 이 때 Local과 Remote에 차이가 발생했을 경우 git pull origin main/develop으로 당겨오기
- 이후 git push --tags를 이용하여 태그까지 추가하면 완료
