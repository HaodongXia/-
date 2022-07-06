# Git学习

1、创建版本库

```
mkdir learngit
cd learngit
pwd

git init /把当前这个目录变成Git可以管理的仓库

git add readme.txt
git commit -m "添加了一个文件"
```



2、版本回退

```
git status /仓库当前的状态

git diffreadme.txt /查看文件内具体修改什么

git log /查看历史修改记录

git reset --hard HEAD /版本回退:HEAD表示当前版本，上一个版本HEAD^,上上个HEAD^^

git reflog /回到未来
```



3、工作区和暂存区

learngit文件夹就是工作区，而隐藏的.git文件就是版本库，内有一个stage的暂存区和master的分支

add将文件由工作区添加至暂存区

commit将文件由暂存区添加到分支



4、

```
git checkout -- readme.txt /放弃修改

//把readme.txt文件在工作区的修改全部撤销，这里有两种情况：

一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；

一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态

git reset HEAD readme.txt
git checkout -- readme.txt

删除文件
git rm test.txt / 确实要从版本库删除文件

git checkout -- test.txt /删错了，回撤
```



5、远程仓库

由于本地Git仓库和GitHub仓库之间的传输是通过SSH加密的，所以，需要一点设置：

- 创建SSH Key。

  ```
  $ ssh-keygen -t rsa -C "youremail@example.com"
  ```

- 登陆GitHub，打开“Account settings”，“SSH Keys”页面：
- 点“Add SSH Key”，填上任意Title，在Key文本框里粘贴`id_rsa.pub`文件的内容



6、添加远程库

首先，登陆GitHub，然后，在右上角找到“Create a new repo”按钮，创建一个新的仓库：

现在，我们根据GitHub的提示，在本地的仓库下运行命令：

```
$ git remote add origin git@github.com:自己的账户/learngit.git

$ git push -u origin master /本地库内容推送到远程

$ git remote -v /查看远程库

$ git remote rm origin /删除远程库

git clone git@github.com:自己账户/gitskills.git /克隆库

远程库的名字就是origin，这是Git默认的叫法
```

7、分支管理

```
$ git checkout -b dev //git checkout命令加上-b参数表示创建并切换，相当于以下两条命令:
$ git branch dev
$ git checkout dev

$ git branch /查看当前分支

$ git merge dev //当前在master分支，将dev分支合并过来

$ git branch -d dev /删除分支

$ git switch -c dev //创建并切换到新分支（更科学）
```

![截屏2022-07-06 17.11.28](/Users/xiahaodong/Library/Application Support/typora-user-images/截屏2022-07-06 17.11.28.png)

bug分支：修复bug时，我们会通过创建新的bug分支进行修复，然后合并，最后删除；

当手头工作没有完成时，先把工作现场`git stash`一下，然后去修复bug，修复后，再`git stash pop`，回到工作现场；

在master分支上修复的bug，想要合并到当前dev分支，可以用`git cherry-pick <commit>`命令，把bug提交的修改“复制”到当前分支，避免重复劳动。



强行删除分支：未合并的分支

```
$ git branch -D 分支名
```

- 查看远程库信息，使用`git remote -v`；
- 本地新建的分支如果不推送到远程，对其他人就是不可见的；
- 从本地推送分支，使用`git push origin branch-name`，如果推送失败，先用`git pull`抓取远程的新提交；
- 在本地创建和远程分支对应的分支，使用`git checkout -b branch-name origin/branch-name`，本地和远程分支的名称最好一致；
- 建立本地分支和远程分支的关联，使用`git branch --set-upstream branch-name origin/branch-name`；
- 从远程抓取分支，使用`git pull`，如果有冲突，要先处理冲突。

8、标签管理

```
$ git tag <tagname> /打标签
git tag -a <tagname> -m "blablabla..." // 指定标签信息
git tag // 查看所有标签

默认标签是打在最新的commit上，如果想打在之前的commit，先用git log，找出commit id，然后再打标签
```

- 命令`git push origin <tagname>`可以推送一个本地标签；
- 命令`git push origin --tags`可以推送全部未推送过的本地标签；
- 命令`git tag -d <tagname>`可以删除一个本地标签；
- 命令`git push origin :refs/tags/<tagname>`可以删除一个远程标签。