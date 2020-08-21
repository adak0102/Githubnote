### 깃헙 강의 day 2 

#### 배포

> 새로운 에디터 깔기 : vs code  (html editor 위해)

>  깃 : 폴더단위 관리 : 해당폴더를 깃으로 관리하게 됨 

> 새로운 프로그램 설치할때
>
> gitbash 껐따 켜줘야함





> mkdir homepage
>
> cd homepage
>
> code (해당 경로/  프로그램 실행)
>
> code 현재폴더 (.)
>
> `code . `  : 현재 폴더 실행됨

> **[vs code]** 
>
> 항상 프로젝트 마다 `README.md` 만듬  (프로젝트 설명서로)  : vs code에 

> git으로 관리 시작 
>
> `git init`
>
> ls -a 해서 .git 있는지 확인 

> 파일 추가 행위 
>
> `git add .` : 현재폴더의 모든 변경사항 더함 
>
> git status 로 확인
>
> 저장하고 commit
>
> `git commit -m "Add README.md"`  = "first commit"  (알아듣기 쉬운)
>
> 구글링 git commit message convention  : 좋은 git commit 메세지 위한 (소통위해 회사에서 필요)
>
> git log 로 컨벤션 확인 
>
> github에 업로드함



> <github pages 활용하기 >
>
> repository name에 페이지 못씀 , github pages 활용하기 
>
> 깃헙이 제공하는 호스팅 기능:  Hosted directly from your [GitHub repository](https://github.com/). 
>
> >  규칙이 있음
> >
> > > 깃헙 username.github.io
> > >
> > > `SungheePark.github.io`   > 오타없이 **reposiroty 네임**에 꼭 이 양식으로 씀!!
> > >
> > > 

> **로컬정보를 원격에 저장**하려면
>
> git remote add origin(첫저장소 보통 )  주소 붙여넣기
>
> `$ git remote add origin https://github.com/adak0102/adak0102.github.io.git`
>
> 확인 : git remote -v    
>
> ($ git remote remove origin : 오류 떴을때 origin  삭제 방법)
>
> git push origin master

vscode 에 새파일 만들기

index.html : 꼭 이대로 (규칙임)



``` 
i@DESKTOP-CS5B0E0 MINGW64 ~/homepage (master)
$ git add index.html

i@DESKTOP-CS5B0E0 MINGW64 ~/homepage (master)
$ git commit -m "Add index.html"
[master af709b7] Add index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html

i@DESKTOP-CS5B0E0 MINGW64 ~/homepage (master)
$ git log --online
fatal: unrecognized argument: --online

i@DESKTOP-CS5B0E0 MINGW64 ~/homepage (master)
$ git log --oneline
af709b7 (HEAD -> master) Add index.html
32647d5 (origin/master) Add README.md

i@DESKTOP-CS5B0E0 MINGW64 ~/homepage (master)

```

> vs code에서 
>
> README.md 
>
> index.html만들고  ! tab 누르면 바로 html 양식 뜸 



> **오류 해결**
>
>  다시  " **자기 유저 네임 adak0102**로 페이지 소스 만들어야함"
>
> $ git remote remove origin
>
> git status
>
> git add . 
>
> git commit -m "modified"
>
> git push origin master
>
> url `adak0102.github.io`열면 페이지 나옴
>
> 



> static <-> dynamic 웹페이지
>
> static 웹사이트
>
> 
>
> dynamic 웹사이트



> 수집, 분석
>
> 수집 ,,가공,,자동화,, 보여주는 유저 친화적 사이트 
>
> 데이터 사이언티스트,에널리스트 : 웹서비스 만드는 능력 필요
>
> 크롤러 (자동), 분석 스트리밍 보여줌
>
> 풀스택
>
> 수집가공분석보여줌 

>저장소 custom domain 부분에서 
>
>자기 이름으로 도메인 만들 수도 있음
>
>장고에서 만든 거 연결

> cd.. 홈디렉토리로 올라감 



> cd..
>
> mkdir website
>
> cd website
>
> 초보몽키 사이트
>
> gatsby 쓰면  동적으로 보이게 됨
>
> 라프텔 회사 
>
> 호갱노노
>
> bit.do/t2_bigdata



> boottstrap  
>
> 내용 복사해서 사용자 i website에 붙임



> git init으로 폴더 master관리 
>
> git add . 
>
> git commit  -m "first commit"

git remote add origin  

git push origin master





code .





로컬에서 변경한거 

add commit push 





변경하면 add commit push





> 개별 리포마다 소개 html 있을 수 있음 (branch개념 필요)



url(images/about.jpg)



hphk-john



heroku

c9.io

https://github.com/connect-foundation/2019-projectsinfo

https://github.com/kefranabg/readme-md-generator

[ide.cs50.io](http://ide.cs50.io/)  : 컴퓨터 한대 빌린거 , 웹서버 하나 빌림

같이 코딩 가능 옆에있는 사람이랑





> cs50

ls

python --version

 $ pip list

 $ pip install django

$ django-admin startproject campus

 $ ls

 $ cd campus

$ python manage.py runserver **8080**



ctrl c 서버 껏다 킴 

share access 하고 

settings.py allowedhosts =['*']

: ide.cs50.io/adak0102/ide/로 들어감 

https://us-west-2.console.aws.amazon.com/cloud9/ide/4e4072220f4a4159befa50ce7bb842a3?#

https://4e4072220f4a4159befa50ce7bb842a3.vfs.cloud9.us-west-2.amazonaws.com/projectapp/index/

도메인 구매 

gabia

GoDaddy





python manage.py runserver 8080





git init

> > master 생김
> >
> > 