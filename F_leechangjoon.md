깃 시작할 때 git init,
사용자 등록은 git config --global user.(name/email) "..."
레포 주소는 git remote add origin "..."
후 파일 작성 및 편집을 하고,
git add .로 예비 저장소에 올린 후
git commit -m "..."로 로컬 저장소에 저장한다.
그리고 git push origin main 을 통해서 원격저장소로 보낸다.
//main이 아니라 master로 되어있다면, git branch -M main 을 통해 바꿀 수 있다.