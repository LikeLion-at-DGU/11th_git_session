#사용자 등록 방법
git config —global user.name(or mail) "깃허브 이름이나 메일 치기"
#초기화 과정
git init

#github으로 협업하기
upstream: 최종 코드 merge 할 곳
origin: 나의 코드 push 할 곳

#깃허브 협업방법
git clone <개인 원격 저장소 url>
git remote add upstream <중앙 원격 저장소 url>
그 후 항상 잘 되었는지 git remote -v 로 확인할 것

#브랜치
: 기존 코드의 사본으로 만든 독립적ㅇ니 개발 공간
git branch: 로컬 브랜치 목록
git checkout -b <name>: 새로운 브랜치 생성 후 해당 브랜치로 작업 위치 이동
git branch -d <name> : 로컬 브런치 삭제

commit message 통해 작업 내용 유추가 가능해야 함. 컨벤션 규칙 참고할 것s