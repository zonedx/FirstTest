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
git reset --HEAD^ 退回上一个版本
git reset --HEAD 3628164..(commit id)  退回未来版本
git reflog  记录每一次命令