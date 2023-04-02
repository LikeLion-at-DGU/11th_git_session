1. github commit 하기
git config --global user.name <github 아이디>
git config —global user.email <이메일>
git init
git remote add origin <개인 url>
git branch –M main
git remote –v
git add .
git commit –m “feat. 6조 윤수민”
git push origin main

*참고> remote 저장소 관련 각종 명령어
git remote -v : 현재 등록된 리모트 저장소 목록
git remote add <name> <url> : 새 리모트 저장소 추가
git remote remove <name> : 리모트 저장소를 삭제
git remote rename <old_name> <new_name> : 리모트 저장소 이름 변경
git remote set-url <name> <new_url> : 리모트 저장소의 URL 변경
git remote show <name> : 지정된 리모트 저장소의 정보
git remote prune <name> :  지정된 리모트 저장소에서 더 이상 존재 않는 브랜치 제거


2. github 협업하기
git clone <fork 한 개인 원격 저장소>
git remote add upstream <중앙 원격 저장소>
git remote add origin <fork 한 개인 원격 저장소?>
git remote - v
ls
cd <cd로 작업할 디렉터리>

git checkout -b B_ysm

gid add .
git commit -m<커밋메세지>
git push origin <brach-name>

-> commit / push 완료!


