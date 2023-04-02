•git 레포 활용법
    바탕화면 > Workspace 폴더에 파일 생성
    파일 우클릭 > code로 열기
    새 파일 생성

•터미널 띄우기
    터미널 > 새 터미널
    터미널 우측 상단에서 git bash로 변경

•git 협업
    git init :초기화
    주소 fork하기
    git clone 개인 원격 주소
    git remote add origin 개인 원격 저장소
    git remote add upstream 중앙 원격 저장소
    git remote -v (확인)

•브랜치 생성
    git checkout -b 트랙이니셜_이름이니셜
    생성 후 트랙이니셜_이름.md 파일 생성
    개인 원격 저장소에 commit/push

•개인 원격 저장소에 올리기
    git add .
    git commit -m <커밋메세지>
    git push origin <브랜치 이름>
    이후 중앙 원격 저장소에서 compare & pull request 눌러서 요청 (깃허브에서)
