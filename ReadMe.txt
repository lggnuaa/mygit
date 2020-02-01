Init github!

ssh-keygen -t rsa -C "lggnuaa@163.com"

git branch


git 命令：
添加修改到暂存区：git add
提交到分支：git commit -m "common"
查看log：git log
		 git reflog
丢弃修改：git checkout -- file		“修改未add到暂存区的撤销方法”
		  git reset HEAD file		“修改已经add到暂存区，但并未commit的撤销方法”
把版本回退到上一个版本：git reset --hard HEAD^  “回退到上上一个版本再加一个^”
回退到某个固定版本：$ git reset --hard <版本号>	 “版本号可以同过git log或git reflog命令查看”
查看分支：git branch
创建分支：git branch <name>
切换分支：git checkout <name>或者git switch <name>
创建+切换分支：git checkout -b <name>或者git switch -c <name>
合并某分支到当前分支：git merge <name>
删除分支：git branch -d <name>
关联一个远程库：git remote add origin git@server-name:path/name.git
本地推送到远程：git push origin master