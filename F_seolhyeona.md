Git?
: 하나의 프로젝트 진행시에 여러 사람의 협업을 도움

<git의 구조>
- Working Directory 
    -> add
- Index(Staging)
    -> commit
- Local Repository
    -> push
- Remote Repository

<git 흐름 _ with 명령어>
1. git remote add origin <url 주소> ; 개인원격저장소
2. 파일 작성
3. git add . ; 전체 파일
4. git commit -m [커밋메시지]
5. git push origin [branch명] ; 개인원격저장소


<협업>
1. 중앙원격저장소 fork -> 개인원격저장소 생성
2. branch 생성
3. 개인원격 저장소에 commit/push
4. Pull Request 버튼 ; 중앙원격저장소에 반영 요청