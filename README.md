# 깃배시를 사용하여 커밋하는 방법을 실습한 코드를 정리해보았습니다
## cd 위치이동
##  .. 그전 위치로 
## git add . 변경된것 다 
##  pwd 현 위치
## git --version  버전확인
## git init 초기화
## git remote add origin 레퍼주소  레퍼와 연결 
## git commit -m "read" 메세지 남김
## git push origin master 깃헙과 연동해 
bash: /c/Users/장세환/.profile: is a directory

장세환@DESKTOP-60V1R5B MINGW64 ~
$

장세환@DESKTOP-60V1R5B MINGW64 ~
$ git --version
git version 2.26.2.windows.1

장세환@DESKTOP-60V1R5B MINGW64 ~
$ git config --global user.name "jang"

장세환@DESKTOP-60V1R5B MINGW64 ~
$ git config --global user.email "jjsst5@nate.com"

장세환@DESKTOP-60V1R5B MINGW64 ~
$ git config --list
credential.helper=manager
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
user.name=jang
user.email=jjsst5@nate.com

장세환@DESKTOP-60V1R5B MINGW64 ~
$ cd Desktop/

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ ls
'~$타이타닉 데이터 분석 프로젝트 기획.pptx'  '딥러닝 책'/
'Animotica - Video Editor.lnk'*              '사진 - 바로 가기.lnk'*
 desktop.ini                                  사회조사방법론/
'Microsoft Edge.lnk'*                         시계열/
 sql/                                        '자바로 배우는 쉬운 자료구조'/
 Untitled.ipynb                               통분방/
'Windows 10 업데이트 도우미.lnk'*             투자론/
'끝난 수업'/                                  프로그래밍언어/
 논문/                                        합격자소서,포폴/
 데이터마이닝-박헌진교수님/                   회귀분석/

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ git clone https://github.com/Jangsehawn/Computational-statistics.git
Cloning into 'Computational-statistics'...
remote: Enumerating objects: 50, done.
remote: Counting objects: 100% (50/50), done.
remote: Compressing objects: 100% (48/48), done.
remote: Total 50 (delta 15), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (50/50), 18.16 KiB | 743.00 KiB/s, done.
Resolving deltas: 100% (15/15), done.

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ cd Computational-statistics/

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/Computational-statistics (master)
$ git add .

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/Computational-statistics (master)
$ git commit -m "readme modified"
[master 3233326] readme modified
 1 file changed, 1 insertion(+)

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/Computational-statistics (master)
$ git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 280 bytes | 93.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Jangsehawn/Computational-statistics.git
   e750281..3233326  master -> master

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/Computational-statistics (master)
$ cd ..

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ cd .

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ pwd
/c/Users/장세환/Desktop

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop
$ cd test1

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/test1
$ git init
Initialized empty Git repository in C:/Users/장세환/Desktop/test1/.git/

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/test1 (master)
$ git remote add origin https://github.com/Jangsehawn/git_test1.git

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/test1 (master)
$ git add .
warning: LF will be replaced by CRLF in .gitignore.
The file will have its original line endings in your working directory

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/test1 (master)
$ git commit -m "text"
[master (root-commit) aae4d3b] text
 3 files changed, 24 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .gitignore
 create mode 100644 .project

장세환@DESKTOP-60V1R5B MINGW64 ~/Desktop/test1 (master)
$ git push origin master

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 617 bytes | 154.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Jangsehawn/git_test1.git
 * [new branch]    
