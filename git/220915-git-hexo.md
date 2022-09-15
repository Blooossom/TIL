# Today I Learned

## 19:00 ~ 21:00

### About Git flow
- 주로 사용할 Branch model
- (hotfix)-master(main)-(release)-develop-(feature)로 구성
- 주니어는 기본적으로 develop-feature에서 개발을 진행

### Git flow process
- 주 process는 https://danielkummer.github.io/git-flow-cheatsheet/index.ko_KR.html에서 확인가능
- 먼저 main branch에서 git_flow_init 커맨드를 사용
> - 몇개의 라인 이후 자동으로 develop branch 생성
> - 또한 자동으로 develop branch로 이동한다.
- git_flow_feature_start_{name}으로 feature 이동
- 작성할 파일 edit후 add>commit
- git_flow_feature_finish_{name}으로 feature 종료
- 이후 develop > release 과정
- git_flow_release_start/finish_{version}로 release까지 완료
- 모두 마쳤다면 push기능을 통해 remote_repo로 보내면 OK
- 이Process를 통해 버전업을 할 수 있음
- 다만 긴급한 문제 > main에서 hotfix branch로 이동하여 바로 작성



## 21:00~22:00

### Github Blog using Hexo

- 과정은 다음과 같다
> 1. hexo설치
> 2. post작성
> 3. hexo generate
> 4. Github에 {username}.github.io라는 새 repo 추가
> 5. deployer설치
> 6. Vim을 이용하여 내부 설정파일 편집
> 7. hexo clean && hexo generate
> 8. hexo server를 통한 local상태에서으 구동 확인
> 9. hexo deploy
> 10. username.github.io에 접속하여 구동확인
