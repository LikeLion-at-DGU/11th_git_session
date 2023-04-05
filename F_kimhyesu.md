section 1 
git의 구조는 크게 둘로 나뉜다
-중앙 원격저장소 : remote repos
=> logcal로 다운 받는 걸 clone , local에서 올리는 걸 push라고 한다 . clone명령어를 시행하면 내 컴퓨터에서 폴더를 다운 받을 수 있다.
   직접 다운 받는 것과의 차이는 clone명령어를 통한 다운은 .git 즉, 예비 저장소에서의 파일이 함께 다운된다.
- 개인원격저장소 :세 개로 나눌 수 있다
(1) 폴더 :내가 흔히 생각하는 컴퓨터 폴더 (2) 예비저장소 : 눈에 보이지 않는다. git이라는 이름으로 저장된다.
=> 폴더에서 예비저장소로 올릴 때는 add : 버전관리에 반영하고자하는 파일을 미리 올려두는 것이다
=> 예비저장소에서 폴더로 갈 때는 reset을 사용함
(2) 예비저장소 (3) local저장소
=> 예비에서 로컬로 가는 건 commit이라고 한다 :실제로 저장소에 저장하는 과정이다.
 (?아마 여기서 local저장소는 내 github일 것이다)

 section 2 로컬에서의 과정
1. git init
2. git remote add origin 내 깃허브 주소 : 이거 두개를 해야 오류가 안난다... 내 깃허브 주소를 origin이라는 별칭으로 사용하게 된다.
3. status 어떤 상태까지 왔는지 확인하는 command
4. add : 실제 폴더에서 예비저장소에 저장하는 .git 파일을 생성해주는 command
5. git commit -m "message" :commit은 내 개인 깃허브 저장소로 올리는 건데 업데이트가 뭐 됐는지 message를 꼭 써주어야 함
6. git branch -M main 

Section 3 로컬과 remote관계로 협업하기
1. git clone <다운받아올 링크> : 실제 내 컴퓨터에 폴더가 생긴다!
2. git checkout -b <브랜치 이름> : main말고 수정이 이루어질 브런치를 생성해주는 것이다
3. git commit -m :메인으로 가보자
4. git merge <합칠 브랜치 이름> : 브랜치에서 작업한 걸 메인 작업대에서 병합해주는 것이다. 