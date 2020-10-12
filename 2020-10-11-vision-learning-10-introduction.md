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

### git是一个版本控制系统
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

安装完成后，还需要给你机器上的仓库指定一个用户名与邮箱地址，用于与他人之间的交互

于是我们对此进行设置，在命令行中输入一下语句（Your name为你的用户名，email@example.com为你的邮箱地址）

	$ git config --global user.name "Your Name"
	$ git config --global user.email "email@example.com"

