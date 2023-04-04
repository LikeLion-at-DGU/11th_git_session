깃허브로 협업하기 - 단체에서 올려준 레파지토리 있으면 포크해서 내 버전 만들기
이 프로그램 열고 작업할 폴더 열어주기
내가 작업할 위치 정해주기 cd (어떤폴더명) 

여기서부터 고대로 적어주기
git clone 내 버전 url
cd (클론 해온 내 폴더명)
git remote add upstream (단체에서 올려준 공식 링크)
git checkout -b (생성할 브런치 이름 정해주기)
git branch : 내 브런치 잘 있나~ 확인해주기


여기서부터는 업로드/새로고쳐서 저장할 때에도

git add .
git commit -m "설명이름인듯"
git push origin (브랜치명)

이후에 깃허브로 이동해서 새로고침 - 새로 뜬 초록버튼 (compare & pull request)
설명 적고 creat pull request 클릭하면 끝..!