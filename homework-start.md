---
layout: default
title: 使用 Git 提交作业
---

# 使用 Git 提交作业
{:toc}

* 目录
{:toc}

## 1、Github What & Why

gitHub 是一个面向开源及私有软件项目的托管平台。作为开源代码库以及版本控制系统，Github拥有超过千万开发者用户，随着越来越多的应用程序转移到了云上，Github已经成为了管理软件开发以及发现已有代码的首选平台。

* 使用 Github，管理你的大学阶段乃至未来你所有的程序代码，观察自己的成长轨迹。
* 使用 Github，组建自己的软件开发团队或加入其他团队，与全球伙伴协同开发有趣的软件。
* 使用 GitPage，作为文档托管空间，介绍你的项目、记录与分享技术学习经验。
* 你也可以建立你的专业博客，突出作为计算机专业学生的优势。

## 2、Github 环境准备

### 2.1 注册 Github 账号

进入 [github ⽹站](https://github.com/) 注册⼀个⾃⼰的账户

`https://github.com/your-account` 就是你 Github 的首页。你所有的文档、代码及其历史都保存在其中的仓库（Repositories
）中。


### 2.2 安装 git 管理⼯具

从 [git 工具官⽹](https://git-scm.com/downloads) 直接下载安装程序，按提示选择合适系统安装。

![](images/homework-helper/git-download.png)

**windows 用户**

安装完成后，在开始菜单⾥找到“Git”->"Git Bash"，点击跳出类似命令⾏的窗⼝（[MinGW](http://mingw.org/)），说明安装成功！

![](images/homework-helper/git-bash-window.png)

这是一个简单的 Unix bash，常用的 Unix 命令都能执行。

* 命令 `git --version` 显示 git 工具的版本
* 命令 `cd ~` 进入用户根目录

**Mac 用户**

期待你的补充

**Linux 用户**

期待你的补充

### 2.3 配置 git 用户

打开 git bash 工具与密码

**配置访问服务器的用户**

```
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```

注意：邮箱必须与 github 注册邮箱一致

**配置访问服务器密码，免去每次提示**

检查是否是用户根目录，如不是输入 `cd ~`

创建 `.git-credentials` 文件，配置访问 github 的用户与密码。例如： 

```
$ echo "https://user:password@github.com" .git-credentials
$ cat .git-credentials
$ git config --global credential.helper store
```

## 3、安装 vscode






