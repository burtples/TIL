# GIT 기본적인 사용법

## Git의 영역

- Working Directory
- Staging Area
- Repository


## Git 명령어

- git add = staging area로 파일 추가
  - untracked --> tracked
  - 기존파일 수정 시 modified로 표시
- git commit = repository로 파일 추가
- git diff <commit1>  <commit2>
  - 두 커밋에 대한 비교
- `git log --oneline`
  - 커밋에 대한 히스토리 간단히 보기
- git clone <remote_repo_url>
  - local로 복제됨
  - .git 파일도 같이 복제
  - 최초 1회 실행
- git pull
  - remote repo와 동일한 버전으로 다운
  - remote 정보가 필요
  - 이미 git으로 관리되고 있어야함 (.git파일 존재)

## Git 명령어 FLOW

**==`git init`==  : 대상 directory GIT으로 관리 설정!**

### 로컬 저장소에 내려받기

> git clone <repo_주소>	(초기설정)
>
> git pull							(수시로)

### GIT에 push하는 단계

- `git add <파일명>`
- `git commit -m "새로운 메시지"`
- `git status`  ==저장소 변경사항 확인==
- `git remote add origin <주소>`
- `git push origin master`

> init / clone 						: 초기설정 
>
> add -> commit -> push	 :업데이트 때마다

> 