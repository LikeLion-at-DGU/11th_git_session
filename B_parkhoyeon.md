git 사용법


* 개인 레포지토리
1) 바탕화면 > Workspace > git 폴더 생성
2) github 사이트에 새 레포지토리 생성
3) 터미널 통해 사용자 등록
$ git config --global user.name [깃허브 아이디]
$ git config --global user.email [깃허브 이메일]
4) 초기화 설정
$ git init
5) 개인 Repository 주소 copy하기
6) 개인 원격 저장소(2에서 만든 거) 연결
$ git remote add origin [개인 원격 저장소 url]
$ git branch -M main (master로 설정된 branch를 main으로 바꾸는 것)
$ git remote -v (개인 레포지토리와 연결 잘 되었나 확인)


* 커밋 하는 법(레포지토리에 올리는 법)
$ git add . (현재 코드 전체 내용을 추가한다는 뜻)
$ git commit -m "원하는 문구" (커밋에 메세지 남기는 것)
$ git push origin main(main 브랜치에 보낸다는 것)


* github으로 협업하기
1) 프로젝트의 중앙 원격 저장소(레포지토리) 생성 -> 가장 중심이 되는 누군가가 해놓았을 것
2) 해당 중앙 원격 저장소를 fork(복제)해 '개인 원격 저장소(레포지토리)' 생성
3) git clone으로 로컬 저장소(내 노트북) 생성 > clone 후 디렉토리 설정
$ git clone [개인 원격 저장소 url]
$ git remote add upstream [중앙 원격 저장소 url]
4) upstream(중앙 원격 저장소) / origin(개인 원격 저장소) 설정
$ cd [작업할 디렉토리]
$ git remote -v (현재 등록된 리모트 목록 확인)
$ git remote add origin [개인 원격 저장소 url]
$ git remote add upstream [중앙 원격 저장소 url]
5) 브랜치 생성
cf 브랜치란?: 기존 코드의 사본으로 만든 독립적인 개발 공간
$ git checkout -b [브랜치 이름] (새로운 브랜치를 생성하고, 해당 브랜치로 작업 위치 이동)
6) 브랜치에서 작업 후 개인 원격 저장소(레포지토리)에 commit/push
$ git add .
$ git commit -m [커밋 메세지]
$ git push origin [브랜치 이름] => 해당 브랜치가 갈라져 내가 작성한 코드들이 그쪽으로 연결됨
7) Pull Request(PR)로 중앙 원격 저장소에 반영 요청
git 사이트에서 'Compare & pull request'버튼 후 내용확인 하고, 중앙 레포에 올려도 되는지 요청 보내기
8) PR 리뷰 후, 오류 없는 코드를 중앙 원격 저장소 관리자가 merge => 관리자가 하는 일
9) 로컬 저장소(내 컴퓨터)의 main 브랜치에서 upstream의 최신 코드 받아오기
=> 최신 상황 업데이트 받고 충돌을 줄이기 위해
10) 예전 브랜치 삭제, 새로운 브랜치 생성 후 작업
=> main 브랜치가 결정되고 중앙에서도 원하는 방향일 때