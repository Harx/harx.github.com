---
title: Git
---

[Pro Git](http://git-scm.com/book/zh/)

~~~
添加远程分支

git remote add origin 
git remote add asmld 


分支的新增与合并

// 新建分支 并切换
git checkout -b feature_x

// 新建远程分支到本地
git checkout -b test origin/test

git branch -r // 查看远程分支
git checkout master // 切换回主分支

// 除非你将分支推送到远端仓库，不然该分支就是不为他人所见的：
git push origin 
git push [远程名] [本地分支]:[远程分支]

// 删除分支
git branch -d feature_x

// 删除远程分支
git push [远程名] :[远程分支]

// 在合并改动之前，你可以使用如下命令预览差异
git diff 

// 用test分支上的file替换当前分支的
git checkout test -- filename

// 合并其他分支到你的当前分支（例如 master）
git merge 


标签

// 创建一个叫做 1.0.0 的标签
git tag 1.0.0 1b2e1d63ff
git log // 获取提交 ID


撒销

// 撒销掉本地改动
git checkout -- 

// 假如你想丢弃你在本地的所有改动与提交，可以到服务器上获取最新的版本历史，并将你本地主分支指向它
git fetch origin
git reset --hard origin/master

// 撒销一个合并
git reset --hard HEAD
~~~
