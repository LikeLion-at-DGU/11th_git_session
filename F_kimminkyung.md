github 협업 시, 그 과정은 다음과 같이 크게 4단계로 나눠진다.
1. 중앙레포에서 fork
2. 브랜치에서 작업
3. 개인레포에 push
4. PR 리뷰 후 merge

먼저, 새 터미널과 Git Bash 기본 설정을 해준다.
1단계에서는 git config --global user.name/email을 통한 사용자 등록과 git init을 통한 초기화 과정이 필요하다.
fork해온 개인 레포를 git remote add origin을 통해 연동해준 후 main을 새로 만들어 덮어쓴다.
git clone, git remote add upstream을 통해 각각 개인레포, 중앙레포를 연결해준다.
2단계에서 git checkout -b를 통해 브랜치 생성 후, 파일을 생성을 하고 작업을 하면 된다. (꼭 저장하기!!)
3단계에서 git add ., git commit -m, git push origin을 통해 개인레포에 push한다.
여기서 커밋메세지의 규칙을 통해 간략, 정확하게 정보전달이 가능하다.
마지막으로, 4단계에서 PR 리뷰 후 관리자가 merge하면 중앙레포에 반영이 된다.
이러한 단계들 이후에는 git checkout main, git pull upstream main을 통해 최신화를 하고 예전 브랜치는 삭제한다.