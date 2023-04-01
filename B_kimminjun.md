git - 소스 이력 추적을 위한 버전 관리 시스템
github - git 프로젝트를 관리하는 저장소 제공

레포 생성 후 최초 1회 해야할 것
1. git 사용자 등록
git config --global user.name "samdolls"
git config --global user.email "minjoon927@gmail.com"
2. 생성한 원격저장소에 연결
git init : 초기화 과정, .git 폴더 생성
git remote add origin 레포 주소
그 후 반복(working directory -> 개인 원격 저장소)
3. 파일 작성 및 편집 후 저장
4. git add . : 디렉토리 내에 있는 변경된 파일 전체를 예비 저장소(staging)에 저장
5. git commit -m "커밋 메세지" : staging에 있는 변경 결과를 로컬 저장소에 commit(추가)
6. git push origin main : 로컬 저장소에 있는 결과를 push하여 원격 저장소에 반영

협업하기 위한 방법
1. 프로젝트의 중앙 원격 저장소(레포) 생성
2. 해당 중앙 원격 저장소에서 fork를 하여 개인 원격 저장소 생성
3. git clone으로 로컬 저장소 생성
git clone <개인 원격 저장소 url>
4. upstream(중앙 원격 저장소) / origin(개인 원격 저장소) 설정
git remote add upstream <중앙 원격 저장소 url>
5. 브랜치 생성
git checkout -b <이름>
6. 브랜치에서 작업 후 개인 원격 저장소에 commit -> push
7. Pull Request(PR)로 중앙 원격 저장소에 반영 요청
8. PR 리뷰 후, 오류 없는 코드를 중앙 원격 저장소 관리자가 merge
git pull <팀원 repo url> <팀원의 작업 branch 이름>
9. 로컬 저장소의 main 브랜치에서 upstream의 최신 코드 받아오기.
git checkout main -> 작업의 위치를 main으로 이동
git pull upstream main -> upstream의 코드 pull 받기
10. 예전 브랜치 삭제, 새로운 브랜치 생성 후 작업