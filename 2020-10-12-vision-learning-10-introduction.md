---
layout: post
title: 视觉教程第十弹：git教程
categories: [vision, course, git]
---

# 视觉教程第十弹：git教程
> 机械是血肉，电控是大脑，视觉是灵魂。

---

# Git 教程
## 一、什么是git

### git是文件的版本控制系统
- 多版本分支
- 多人合作
- 简单低成本的备份及版本回退
- ……
	
## 二、安装git
	
### 在Ubuntu上安装git
打开终端，在命令行输入以下命令即可完成安装

	sudo apt-get install git

### 在Windows上安装git
	
在Windows上使用Git，可以从Git官网直接下载安装程序(https://git-scm.com/downloads)
，然后按默认选项安装即可，此处不做赘述。

安装完成后，在开始菜单里找到“Git Bash”，点击后弹出类似下图所示的类命令行窗口，git便安装完成

![img](https://github.com/void-zxh/RM/blob/master/image/1.JPG) 

之后，还需要给你机器上的仓库指定一个用户名与邮箱地址，用于与他人之间的交互

于是我们对此进行设置，在命令行中输入一下语句（Your name为你的用户名，email@example.com为你的邮箱地址）

	git config --global user.name "Your Name"
	git config --global user.email "email@example.com"

注意: git config命令的--global参数，这意味着你这台机器上所有的Git仓库都会使用这个配置，

若想给特定的项目仓库指定单独的用户名与邮箱地址，则可遵循以下步骤

打开项目所在的.git文件夹(隐藏，可通过设置显示)，在此文件夹下打开git命令行窗口
输入以下命令：

	git config user.name  "Your Name"
	git config user.email "email@example.com"

至此，安装git与初步设置的过程就结束了

## 三、git相关功能与命令介绍

git是一种文件版本控制系统，我们可以建立自己的仓库(版本库)，它保留了用户文件编辑中各个版本，具有从远程clone他人开源仓库、往远程仓库上传文件等功能，
接下来，我们将介绍git中的一些基本功能与相关命令

### 创建版本库

#### 什么是版本库

版本库是git实现版本控制的基础。什么是版本库呢？

版本库又名仓库，英文名repository，你可以简单理解成一个目录，这个目录里面的所有文件都可以被git管理起来，每个文件的修改、删除，git都能跟踪，以便任何时刻都可以追踪历史，或者在将来某个时刻可以“还原”。

#### 创建版本库的流程

找到一个想开仓库的地方，打开Git Bash，输入以下命令，新建文件夹，并进入文件目录（repo-name为仓库名）

	mkdir repo-name
	cd repo-name

若不确定当前目录，可查看命令行窗口上目录或输入pwd命令查看
