## github로 협업하기

1) 프로젝트의 중앙 원격 저장소(repository) 생성

2) 해당 중앙 원격 저장소 fork해 개인 원격 저장소 생성
- 중앙 repository 내부에 fork 눌러 개인 repository로 복제

3) git clone으로 로컬 저장소 생성 > clone 후 디렉토리 설정
-- git clone <개인 원격 저장소 url>
-- git remote add upstream <중앙 원격 저장소 url>

4) upstream(중앙 원격 저장소) / origin(개인 원격 저장소) 설정
-- git remote -v => 현재 등록된 리모트 저장소 목록
-- git remote add <name> <url> => 새 리모트 저장소 추가

5) 브랜치 생성 반복

6) 브랜치에서 작업 후 개인 원격 저장소에 commit / push
- 브랜치란 기촌 코드의 사본으로 독립적인 개발공간
-- git checkout -b <name> =>을 통해 브랜치를 생성하고 작업 위치로 이동할 수 있음

7) Pull Request(PR)로 중앙 원격 저장소에 반영 요청
-- git add .
-- git commit -m "커밋메시지"
-- git push origin <branch 이름>

8) PR 리뷰 후, 오류 없는 코드를 중앙 원격 저장소 관리자가 merge

9) 로컬 저장소의 main 브랜치에서 upstream의 최신 코드 받아오기
- 최신화 전, 작업 위치를 main으로 이동 -> git checkout main
- upstrea의 코드 pull 받기 -> git pull upstream main

10) 예전 브랜치 삭제, 새로운 브랜치 생성 후 작업