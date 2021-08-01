# git_useage
git 命令行使用方法


# Git 分支管理
创建分支命令：
git branch (branchname)

切换分支命令:
git checkout (branchname)

创建新分支并立即切换到该分支下：
git checkout -b (branchname) 
 
当你切换分支的时候，Git 会用该分支的最后提交的快照替换你的工作目录的内容， 所以多个分支不需要多个目录。

合并分支命令:
git merge 

$ mkdir gitdemo  
$ cd gitdemo/  
$ git init  
Initialized empty Git repository...  
$ touch README  
$ git add README  
$ git commit -m '第一次版本提交'  
[master (root-commit) 3b58100] 第一次版本提交  
 1 file changed, 0 insertions(+), 0 deletions(-)  
 create mode 100644 README  
 
 列出分支
 git branch

删除分支
git branch -d (branchname)

# Git 查看提交历史

git log - 查看历史提交记录。
git blame <file> - 以列表形式查看指定文件的历史修改记录。
 
# 远程仓库

# git github
 
github创建远程仓库（创建了readme文件）
 
本地命令：
git init 
git add --all
git commit -m 'init'
git remote add origin git@github.com:BenYu2021/xxx.git
 
### 把github远程仓库readme文件合并到本地，远程分支main
git pull --rebase origin main
### 提交到github
git push -u origin main