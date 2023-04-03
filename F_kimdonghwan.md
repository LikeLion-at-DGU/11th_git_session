Git & Github
1.
Git: 소스 이력 추적을 위한 버전 관리 시스템
Github: Git 프로젝트를 관리하는 저장소 제공
2. Git 설치
Window 버전 확인 방법: 시스템 정보를 검색 -> 시스템 종류 (ex) x64 기반 PC)
터미널 활용: window 버튼 -> 
버전 확인, 터미널 -> Git bash -> git ?version 
이력 추적을 위한 이름등록( git config ?global user.name “”
이메일 등록( git config ?global user.email “”)
리스트 등록 잘됬는지 확인하는 법(git config ?list) 빠져나오기 Q
4.Git 구조 
로컬,내가 일하는 컴퓨터( Working Directory(git에서 작업됨)->staging(commit 할 파일의 예비의 저장소)->Local Repository(각 컴퓨터의 git이 관리하는 로컬 저장소 커밋했던 것을 여기다가 저장)
?원격 저장소( Remote Repository -Github)(gitub 등 외부에 위치한 원격 저장소)
5.로컬 Git 저장소 생성
Step 1. Init
Working Directory(내가 작성한 코드들의 파일이 있는곳) 파일들을 관리하려면 Init으로 초기화해야함
(*주의 초기화하려면 나의 프로젝트가 위치한 곳으로 이동후 터미널에서 명령 실행)
Step 2. .gitignore 파일 추가	(파일을 만들어 그 안에 파일은 무시됨)
Step 3. git status 
Step 4. git add . OR Git add “파일명”
(Working Directory ->(add) Stagging)
Step 5. git commit -m “message”
(stagging->(commit) Local Repository)
