Git: 분산 버전 관리 시스템

<시작 - 기본 개인 작업>
1. 깃허브에서 레포지토리 생성
2. 터미널 띄우고 깃배시 설정 후 사용자 등록
git config --global user.name "github_username"
git config --global user.name "github_usermail"
3. 생성한 원격저장소에 연결
git init
git remote add origin [레포주소]
+만약에 master라면.. git branch -M main으로 main으로 바꾸기
git remote -v

# 최초 1회만 시행

4. 파일 작성 및 편집, ctrl+s 바로바로 하기!
5. 파일의 생성 변경 삭제를 index에 추가
git add .
6. 변경 결과 로컬저장소에 commit 추가
git commit -m [커밋메시지]
7. 로컬 저장소를 push하여 원격저장소에 반영
git push origin main

<협업하기>
1. 프로젝트의 중앙 원격 저장소 (레포) 생성
2. 중앙 레포 내부에 fork 눌러 개인 레포로 복제
3. 클론 (내 로컬에 저장) git clone <개인 원격 저장소 url>
4. 작업할 디렉토리 설정
ls -> cd ->ls  #필수!!
5. 깃 리모트 설정(중앙원격저장소랑 연결)
git remote add upstream
6. 브랜치 생성 -> md파일 생성
7. 작업 내용을 먼저 개인 레포에 올리기
git add .
git commit -m <커밋메시지>
git push origin <branch-name>
8. 깃허브에서 마무리~