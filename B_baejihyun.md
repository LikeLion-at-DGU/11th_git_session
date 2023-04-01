# Git 협업
### ✔ Git과 Github
- Git : 분산 버전 관리 시스템  
프로젝트의 변경 사항을 시간에 따라 기록하고, 이전 버전과 비교하며 수정 사항을 관리할 수 있음  
- Github : Git 기반의 프로젝트 호스팅 플랫폼  
Git을 이용하여 프로젝트를 호스팅하고 다른 사람들과 공유할 수 있는 기능을 제공함  
Git 프로젝트를 관리하는 저장소 제공

### ✔ Git 구성 요소
- Working Directory (작업 공간)  
현재 작업 중인 프로젝트가 위피한 디렉토리
- Index/Staging (예비 저장소)  
commit 할 파일의 예비 저장소
- Local Repository (로컬 저장소)  
각 컴퓨터의 Git이 관리하는 로컬 저장소
- Remote Repository - Github (원격 저장소)  
외부에 위치한 원격 저장소

### ✔ Git 사용법
1) github에서 Repository 생성
2) 사용자 등록  
```
git config --global user.name "github_username"  
git config --global user.email "github_useremail"
```
3) 생성한 원격저장소에 연결
```
git init
git remote add origin [레포주소]
```
4) 파일 작성 및 편집
5) 파일의 생성 변경 삭제를 index에 추가
```
git add .
```
6) 변경 결과를 로컬 저장소에 commit (추가)
```
git commit -m [커밋메시지]
```
7) 로컬 저장소를 push하여 원격 저장소에 반영
```
git push origin main
```

### ✔ Github로 협업하기
1) 프로젝트의 중앙 원격 저장소 생성
2) 해당 중앙 원격 저장소를 fork 해서 개인 원격 저장소 생성
3) git clone으로 로컬 저장소 생성 -> clone 후 디렉토리 설정
```
git clone <개인 원격 저장소 url>
git remote add upstream <중앙 원격 저장소 url>
```
4) upstream (중앙 원격 저장소) / origin (개인 원격 저장소) 설정
```
git remote -v 
```
5) 브랜치 생성
```
git checkout -b <name>
```
6) 브랜치에서 작업 후 개인 원격 저장소에 commit/push
7) pull Request(PR)로 중앙 원격 저장소에 반영 요청
8) PR 리뷰 후, 오류 없는 코드를 중앙 원격 저장소 관리자가 merge
9) 로컬 저장소의 main 브랜치에서 upstream의 최신 코드 받아오기
10) 예전 브랜치 삭제, 새로운 브랜치 생성 후 작업