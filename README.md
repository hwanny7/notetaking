# 7월 15일

**GIT 사용 방법**

1. 새 폴더를 생성한다.
2. 오른쪽 마우스 클릭 > git bash here
3. code . 으로 visual studio code 를 열기
4. git init 로 저장소를 초기화 한다.
5. touch newfile.txt 또는 newfile.py 등 파일을 생성
6. 파일 안에 내용을 작성하고 저장
7. git add(파일이름) 또는 git add . 등 지금까지 작업한 내용을 staging area 에 저장한다.
8. git commit -m "원하는 이름" 으로 commit 한다.

working directory: 내가 작업하고 있는 디렉토리
staging area: 특정 버전으로 관리하고 싶은 파일이 있는 곳 (git add를 하면 staging 파일에 올라간다)
repository: 커밋이 저장되는 곳
---
**git command**
rm -rf .git (깃을 삭제하는 명령어. 실행하면 master가 사라진다)
git init (저장소 초기화. master를 생성한다.)
git add<filename>
git add . 
git commit -m "title"
git status
touch title.파일형식
git log (지금까지 생성된 commit의 로그 확인)
---
**깃허브 연결 방법**

1. 새로 만들 때
echo "# my_repo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/hwanny7/my_repo.git
git push -u origin main

2. 기존 파일과 연결할 때
git remote add origin https://github.com/hwanny7/my_repo.git
git branch -M main
git push -u origin main

## 여러가지 팁
1. 깃 허브에서 원격으로 수정하면 local이랑 원격의 commit 내용이 달라져서 충돌이 일어날 수 있음. (깃 허브에서 수정은 가능하지만 웬만하면 local 에서 하는 것을 권장함.)
2. 외부에서 깃허브로 push하고 집에 가서 clone으로 복사해서 사용할 수 있음
3. 친구를 초대해서 파일을 공유할 수 있음
4. public 으로 되어 있는 git 은 pull로 가져올 수 있지만, 권한이 있는 사람만이 수정해서 push 할 수 있음




