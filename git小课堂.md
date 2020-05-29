# git小课堂

## git的基本介绍

* `SVN`是一个集中式版本管理系统。
* `git`是一个分布式版本管理系统，由linus开发。
* 分布式和集中式的区别
  * 集中式
    1. 指的是版本库放在服务器上，干活就得先从服务区上拉取代码，干完活就得推送到服务器上。
    2. 必须联网。如果服务器上代码库出现问题，所有人没法干活。
  * 分布式
    3. 指的是版本库在每个开发的本地电脑上，干活只需推送到自己本地的代码库中。
    4. 每个开发本地有一个完整的代码库。

## git配置

* 直接在git官网下载安装包安装
* 配置账号和邮箱
  
```shell
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
```

* 初始化仓库

```shell
git init
```

* 一般仓库中有一个隐藏的文件`.git`，如果没有表示该文件夹不是`git`仓库。执行`git init`即可。我们远程克隆的仓库会有该文件夹。

## git的workspace stage/index respository remote的理解

* `workspace`工作区指的是我们本地的文件夹
* `stage`暂存区指的是我们执行`git add`操作后的临时仓库
* `respository`指的是我们执行`git commit`操作后的仓库，也叫版本库。
* `remote`指的是我们执行`git push`后的托管服务器，我们现在用的`gitlab`就是`remote`。

## git常用操作

```shell
git init
git clone
git config
git add -A / git add -fielname
git commit -m 'desc'
git status
git diff
git log
git checkout
git branch
git pull
git merge
git fetch
git cherry-pick
git rebase
git stash
```

## git可视化工具介绍

`SourceTree` `GitLens + Git Graph`

## 工作中常用的git小知识