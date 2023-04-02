git init : 초기화
 git add : 내 프로젝트 중 버전관리될 파일을 지정
 git add. : 전체를 add / git add "파일명" : 파일만 add
 git rm/reset : 잘못 add 한 것을 되돌려줌
 git commit -m "커밋에대한정보" : staging 에서 local repository로 이동시키기 위한 작업 / 로컬저장소에 변동기록을 남기기 위해 commit을 실행한다
 git bracnch -M main : 현재 브랜치의 이름을 main으로 변경한다 / 브랜치 : 독립된 작업환경 , 메인 : 메인작업공간이기에 이곳에서 작업을 지양한다
 gitgit remote add origin <원격저장소 주소>

: 로컬저장소에 저장된 폴더를 원격저장소로 보내기 위해, 원격저장소를 지정한

git push -u origin main : 초기에??

git push : 브랜치 내 내용을 원격저장소로 보낸

원격저장소로 프로젝트를 푸시하면 깃허브에서 코드 확인이 가능

협업

git clone <원격저장소주소>

원격저장소에서 프로젝트를 내 로컬환경/컴퓨터로 가져올 때 사용하는 명령

→ 코드 주소 카피 

git checkout -b <브랜치명> : 새 브랜치 이름 설정해서 만들어주는 동시에, 그 브랜치로 이

git checkout <브랜치명>

: 메인에서 빠져나와 브랜치에서 작업을 하는 거쥬.

git commit -m : ????

git checkout main : 메인으로 돌아가요

git merge 브랜치명 : 변경사항을 한 줄기로 합쳐줄 때 명령어 

→ 브랜치 내에서의 변경사항을 메인으로 옮기기