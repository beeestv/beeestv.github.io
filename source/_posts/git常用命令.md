---
title: git常用命令
date: 2018-08-11 23:04:22
tags:
---

### 常用命令

git checkout -- XX 把XX文件在工作区的修改全部撤销。
git rm XX 删除XX文件
git remote add origin https://github.com/tugenhua0707/testgit 关联一个远程库
git clone https://github.com/tugenhua0707/testgit  从远程库中克隆
git checkout –b dev  创建dev分支 并切换到dev分支上
git branch  查看当前所有的分支
git fetch origin develop:develop 拉取远程的develop分支，并在本地创建一个develop分支与之匹配
git checkout master 切换回master分支
git merge dev    在当前的分支上合并dev分支
git branch –d dev 删除dev分支
git branch XX  创建分支
git remote 查看远程库的信息
git remote –v 查看远程库的详细信息
git push origin master 把当前分支推送到远程分支上
<!-- more -->

mkdir XX 创建一个空目录，目录名为XX
pwd 显示当前目录的路径
cat XX 查看XX文件内容
git init 把当前的目录变成可以管理的git仓库，生成隐藏.git文件
git add XX 把xx文件添加到暂存区去，支持正则匹配批量添加文件，如git add .添加所有文件
git config -l 查看config信息
git config --global user.name "xxx"
git config --global user.mail "xxx"  配置用户名和邮箱
git commit –m "" 提交文件，–m后面的是注释，注释是必要参数
git status 查看仓库状态
git diff [XX] 查看XX文件修改了那些内容

git log 查看提交历史记录
git log —pretty=oneline  查看简洁历史记录
git log -p 查看文件修改详细对比
git log —stat 查看文件修改行数
git log -<number> 限制显示数量
git shortlog 按作者显示提交情况
git reset  --hard HEAD^ 或者 git reset  --hard HEAD~ 回退到上一个版本(如果想回退到100个版本，使用git reset –hard HEAD~100 )
git reset —hard 版本号 会退到指定版本
git reflog 查看历史记录的版本号id

git stash 把当前的工作隐藏起来，等以后恢复现场后继续工作
git stash list 查看所有被隐藏的文件列表
git stash apply 恢复被隐藏的文件，但是隐藏区内文件不删除
git stash drop 删除文件
git stash pop 恢复文件的同时，也删除隐藏区内的文件

### 相关文章

#### git log高级用法

https://github.com/geeeeeeeeek/git-recipes/blob/master/sources/Git_log高级用法.md?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io  

#### git log 高级用法简洁版

https://git-scm.com/book/zh/v1/Git-基础-查看提交历史 

