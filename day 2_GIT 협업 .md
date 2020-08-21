## GIT 협업 -> 독재 

#### 1. push &pull : 초대가 필요

#### 2. Fork&PR (Pull Request) : 오픈소스 프로젝트 

#### 	(불특정 다수에 열려있는 프로젝트 ex. tensorflow )

#### 3. Shared Repository (현업)

- Git Flow

- Github Flow



# 1 push &pull

  

팀장 

>mkdir wordchain
>
>cd wordchain 
>
>code . 
>
>​		README.md 파일 만듬
>
>​		#끝말잇기
>
>​		#제시어

>git init
>
>git status
>
>git add README.md
>
>git commit -m "start wordchain"
>
>새 repository [wordchain] 만들기
>
>git remote add origin [repository url paste]
>
>git remote -v(확인)  
>
>git push origin master



https://github.com/Joonhong-Park/wordchain



노예 - 자기 컴에 가져오기 

> git clone [url]
>
> cd wordchain
>
> code . 
>
> 끝말잇기 작성후
>
> (add/ commit / push)
>
> git add . 
>
> git commit -m " "
>
> >  *git push origin master*
> >
> > 하면 안됨 >> 허가를 내줘야 가능 
>
> >  **대장** <manage access> 
> >
> > invite a collaborator : 초대해줌 
>
> 메일 초대장 accept 
>
> git push origin master 다시 하면 됨! 
>
> > 대장 
> >
> > git pull origin master
> >
> > 

<pull push scenario>

```
git add.
git commit -m "4"
git push origin master
------------------------
git pull origin master
```







>대장 - 노예
>
>push pull 
>
>동시에 일하지 못한다.
>
>오픈소스로 사용하기 어려움 _  invite 하지 않으면 push 자체가 안됨 ( 코드 기여 안됨 )



# 2 Fork&PR

>tensorflow 
>
>https://github.com/tensorflow/tensorflow/graphs/contributors 
>
>https://github.com/tensorflow/tensorflow/graphs/contributors



> 사차산업빅데이터 8행시
>
> star
>
> gitstar-ranking.com
>
> https://github.com/JaeYeopHan/Interview_Question_for_Beginner  : 기술면접 
>
> Fork
>
> 저장소가 복제됨

> cd..
>
> git clone >>master떠있음(git으로 관리되는 폴더라는 뜻)
> git clone http url
> cd 100day >> master 뜨게 됨
>code . 
>git remote -v


new pull request 

create pull request 



git status

git add README.md



merge pull request해서 합침



> og : 오픈 그래프
>
> 뻥이요



# 3  Shared Repository

- Git Flow

- Github Flow

점검하고 합쳐줌



cd~

mkdir branch

cd branch

git init

touch a.txt

git add a.txt

git commit -m "Add.a.txt"

 

세계를 두개로 나눌 것

Branch 생성 문법

> (1) git branch
>
> 현재 존재하는 branch들을 조회
>
> > 현재 master 밖에 없음 

> (2) git branch [브랜츠명]
>
> 새로운 branch를 생성

> git branch test
>
> git branch
>
> > > 현재 있는 곳 *master로 뜸

git checkout 

> 과거 보러갈때랑 다른 세계 보러 갈때 
>
> git checkout branch

git branch

touch b.txt

git add b.txt

vit commit -m "ADD b.txt"

git log --oneline

ls

git checkout master

ls



**branch 지우기** 

**git branch -d test**

(4) git branch -d [브랜치명]

빈 branch 삭제

git branch -D [브랜치명]

비어있지 않은 commit 이 하나라도 있는 branch를 삭제 





branch 해놓고 하면

원본 건들지 않고 자유롭게

여러사람이 자기의 세계에서 작업





git branch sunny

ls

git checkout sunny

touch b.txt

git add b.txt

git commit -m b.txt

git log --oneline

git checkout master

ls

git merge sunny

**git merge 브랜치 이름 (해당 세계가 현재 세계로 합쳐짐)**

sunny는 아직 살아있음

git log --oneline

ls

**branch는 1회용이다  : 한번 열고 지우는 것 ! 재활용 노노 (1회용 임시작업, 잠시 만들고 태스트 위함_가지 노노)**

**git branch -d sunny**

: 이미 병합된 브랜치라 -d로도 삭제 됨 





>  Git-flow

master브랜치(거의 못건듬): 실제 돌아가는 배민 앱 

develop브랜치 (개발)

login브랜치..

develop-> release (test서버) : 서버 2-3개 정도, 해외,국내,test서버... ->회사마다 QA팀이 점검 ,,,Quality Assurance팀  _ 버전업 하면서 고치고 -> master로 감

hotfix _ 임시브랜치_ 오류날때 위해_ 진짜 중요한 코드 넣어놈 

https://woowabros.github.io/experience/2017/10/30/baemin-mobile-git-branch-strategy.html







> 만든 폴더 삭제
>
> rm -rf collabo 







> collabo
>
> 

https://github.com/connect-foundation/2019-18

collabo파일 만들고 

code.

html/ Readme

gitinit

git add . 

git commit

뉴 리퍼지토리 만듬 collabo

git remote add origin [url]

git push origin master

> 부하 
>
> > git clone [url]
> >
> > 

<각자의 브랜치로 동시 작업 함>

대장

git branch sunny-intro

> > 부하
> >
> > git branch joonhong-intro

git checkout sunny-intro 

<절대 마스터 건드리지 않음_마스터 브린치는 맨 앞에 있음 _브랜치에서 작업함>

팀장 마크다운

노예 html  신경씀 

``` html에 작성 
## 팀소개

- 박성희 : sunny , 마크다운 작성
- 박준홍: 학생, html 작성
```



> 대장 
>
> git add README.md
>
> git commit -m "Add team member info"
>
> > 짝궁 
> >
> > git add html

git push origin sunny-intro 

master 아니라 우리가 가진 branch (원격에 push 할때- 우리가 가진 branch)

> > 짝궁
> >
> > git push origin 짝궁-intro



팀장은 초대 먼저 _ settings_ manage access_invite

git push origin sunny-intro 

code 에 branch 추가 되어있음 

하고 

pull-request 에서 new pull request 

base:master<- compare :sungheepark으로 하고 

pull request





> 코드 리뷰 대장이 함
>
> pull request 에서 merge pull request 후 
>
> delete branch
>
> master껏도 merge 후
>
> branch delete 

https://hpy.hk/github-flow





> 다른 브랜치에서 pull하면 안됨 
>
> https://git-school.github.io/visualizing-git/
>
> master에서 master pull

