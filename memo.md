```sh
pwd
mkdir hello-git
ls
cd hello-git
history
git init
ls # 안나옴
ls -a # .git 숨김이 나옴
git status 
git add
git add .
git status
opencode
```

```
개발자 소개 페이지를, 최소한의 html로만 만들어줘. hello-git에.
```

```sh
# rm -rf .git
git init
git add {파일명:1글자 입력하고 tab}
```

```sh
git reset
git add .
# git status
```

```sh
mkdir test
git status
```

```sh
touch test/test.txt
```

```sh
git status
mkdir app
touch app/.gitkeep
git status
history
```

```sh
git add .
```

- https://github.com/signup

- https://build.nvidia.com/explore/discover
- Get API Key
- 계정 만들기

- email : mkdir261105@gmail.com
- username : sssuphaaa

```sh
git config --global user.name "{username}"
git config --global user.email "{깃허브 가입시 쓴 이메일}"
git config list --global
```

```sh
git commit
# 영어자판 i (편집모드) -> 커밋메시지를 입력 -> esc -> :wq!
git log
git log --oneline
```

```sh
git init # rm -rf .git
git status
# 파일 수정 처리 + 경로만 있을 경우는 인식 X
git add . # 일괄 추가
git status
# git commit # i -> 커밋 메시지 -> esc + :wq! / esc + :q!
git commit -m "{메시지}"
```

```sh
@index.html About 아래의 소개를 AI 엔지니어를 중심으로 64자로 작성해줘. 추가 수정은 금지.
```

```sh
git status # 파일의 변경여부 Y/N
git diff # 파일의 변경여부 상세
# q 혹은 :q
```

```sh
git commit -m "please use ollama ai"
# git commt -m "please use ollama ai"
# git commit m "please use ollama ai"
# git commit -m "please use ollama ai
git log --oneline
```

```sh
git commit --amend -m "{수정할 메시지}"
git log --oneline
```

```sh
git revert {취소할 커밋}
# 040fcb4 -> 040f
# esc -> :wq! / q!를 했을 경우에는 취소되지 않음 (기본값으로 revert 해줌)
```

```
hello-git에 있는 .gitignore 일반적으로 들어가야할 모든 규칙을 넣어줘.
```

```sh
git add .
# soft면 스테이징도 그대로 두고 특정 위치로 감
git reset --soft
# mixed면 스테이징까지 특정 위치로 감
git reset # git reset --mixed
# hard면 워킹 디렉토리까지 특정 위치로 감
git reset --hard
```

```sh
git reset --mixed HEAD
```

```sh
touch something.txt
git add .
git commit -m "st"
# 커밋까지 한 것
touch anything.txt
git add .
# 스테이징만 한 것
touch nothing.txt
# 워킹 디렉토리만 영향을 받음
```

```sh
git reset --soft HEAD~1
# something
git reset --mixed HEAD~1
# staging까지 다 밀림 + 파일은 살아있음
git reset --hard HEAD~1
# 해당 커밋에서 staging 되었던 것을 아예 워킹 디렉토리에서도 삭제
```

```sh
clear
```

- https://github.com/new
- https://github.com/sssuphaaa/mermaid

```sh
git remote -v
git remote add origin https://github.com/sssuphaaa/mermaid
# 1. add -> ad, addd, dd
# origin -> rigin, origi, orign
# github~, merma
# 1) 다시 하면 됨
# 2) origin은 등록 안됐으니까 괜찮다 # git remote remove orign
# 3-1) git remote remove origin 
# 3-2) git remote set-url origin ~
```

```sh
# git remote
git remote -v
```

```sh
git branch -M main
git push origin main
# git push -u origin main
# origin 원격저장소 이름과 main 브랜치(버전) 이름을 생략해도 바로 push
```