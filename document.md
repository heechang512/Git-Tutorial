#### Git 설치 및 사용법 익히기 [Git으로 시작하는 협업] ####

git

git --version

makedir c:\Education

cd c:\Education



git config --global user.name heechang512

git config --global user.email lee.heechang@yahoo.com

git clone https://github.com/heechang512/Git-Tutorial.git





**Git-Tutorial **







**reference :**

https://github.com/heechang512/Git-Tutorial.git

**…or create a new repository on the command line **

echo "# heechang512" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/heechang512/Git-Tutorial.git
git push -u origin main

**…or push an existing repository from the command line **

git remote add origin https://github.com/heechang512/Git-Tutorial.git
git branch -M main
git push -u origin main

**…or import code from another repository **

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

[Import code](https://github.com/heechang512/heechang512/import)



**[Github] Github에서 Repository 삭제하기**

1. Github에서 삭제할 repository을 선택.

2. 파일이 있는 페이지로 이동.

3. 상단에 [Settings] 를 선택 합니다.

4. 아래로 쭈욱 스크롤하여 맨 마지막에 **Danger Zone** 이 나온다.

5. [Delete this repository] 버튼을 틀릭 합니다.

6. Confirm을 해주고 (패스워드 와 삭제할 repository name을 입력) 나면 삭제 됨.

   ​

**[Git] 깃허브 commit 삭제하기**

$git reset <옵션> <돌아가고싶은 커밋 지점>

옵션에는 3가지 종류가 있다.

1. --hard : 돌아가려는 지점 이후 모든 내용 삭제.


2. --soft : 돌아가려는 지점으로 돌아가지만 해당내용은 남아있으며 인덱스도 그대로 있다.


3. --mixed : 옵션을 생략하면 mixed로 설정되며, 돌아가려는 지점으로 돌아가지만 인덱스는 초기화 된다.

$git reset --hard d075bf9
$git push -f origin master