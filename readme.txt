Git is a version control system.
Git is free software.

mark:
git init 把当前目录变成可管理的仓库
git add <file>  可重复使用 添加多个文件
git commit -m "xxx" 提交
git status  查看仓库当前状态
git diff 查看文件具体修改了什么内容

git log  查看历史记录
git log --pretty=oneline
git reset --hard head^ 退回上一个版本
git reset --hard 3628164..(commit id)  退回未来版本
git reflog  记录每一次命令
git diff HEAD -- readme.txt  可查看工作去和版本库里面最新版本的区别
git checkout -- readme.txt  把readme.txt文件在工作区的修改全部撤销（回到最近一次git commit 
或git add时的状态）
git reset HEAD file 把暂存区的修改撤销掉，重新放回工作区

ssh-keygen -t rsa -C"youremail@example.com"  创建SSH key
git remote add origin git@github.com:[帐户名]/[仓库名].git  关联github远程库
如果创建远程仓库的时候 自动创建了README文件，那么推送的时候会报错  需要先合并：
git pull --rebase origin master
git push origin master  把当前分支master推送到远程

git checkout -b dev  创建并切换到dev分支
==这两条命令（git branch dev  git checkout dev）
git merge [branch name ]合并指定分支到当前分支
git branch -d[name] 删除分支
