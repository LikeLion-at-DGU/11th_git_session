[Git session에서 배운 내용 요약 정리]

Git = 분산 버전 관리 시스템
Github : git 프로젝트를 관리하는 저장소 제공
Git의 구조에는 Local 환경과 Remote 환경이 있다
내가 작업하고 있는 환경 Local
- working directory : 내가 작업하고 있는 코드, 파일들이 있는 곳
- 여기서의 이력을 관리하려면 init 명령어, 초기화를 시켜줘야 한다
- 나의 프로젝트가 위치한 곳으로 이동 후 터미널에서 명령 실행

Github에 소스 반영하기
$ git remote add origin <원격저장소 주소>
- Local 이라는 내 저장소에서 벗어나 github 외부에 저장
- github에서 저장소를 만들고 등록하는 명령어가 $ git remote add origin 명령어다

Local Repository --> push --> Remote Repository - Github

Github으로 협업하기
push해서 업로드를 했기 때문에, 이걸 갖고 어떻게 협업을 하는지 한번 보도록 하자

$ git clone <원격저장소 주소>
- 협업을 위해서는 원격저장소에서 그 프로젝트를 local 환경, 내 컴퓨터로 가져와야 한다

$ git checkout -b <브랜치명>
- Branch를 설정할 수 있는 checkout 명령어를 보자
- Main이라는 중심 줄기에서 벗어나서 새로운 가지를 만든다

$ git commit -m ...
- branch에서 작업을 마친 후에 commit을 하면 작업사항을 main으로 반영하는 일만 남았다
- 이 작업은 commit이라는 명령어로 수행을 한다. 합치는 작업, 병합하는 작업을 이행하기 위해서는 다시 main으로 가야한다