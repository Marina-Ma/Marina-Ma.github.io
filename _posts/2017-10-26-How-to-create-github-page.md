---
layout: post
title: How to create GitHub page
date: 2017-10-26 17:00:00 +0300
description: 用GitHub管理文章的版本，用GitHub page作为Blog，自动发布文章。只享受写作的过程，让写作飞起来！ # Add post description (optional)
img: how-to-start.jpg # Add image post (optional)
tags: [Productivity, Software] # add tag
---

GitHub是Git+Hub的组合。那什么是Git呢？Git是分布式版本控制系统，GitHub正是基于Git开发的。

### 为什么要用GitHub写Blog
1. 版本控制，写论文就能体现出GitHub的优点了，当年怎么没发现呢？！
1. 掌握Github用法，为以后学习计算机语言打下基础。
1. 用Markdown语法写的Blog，也很方便移植到微信公众号里。

如果扩大到一家企业的知识管理，先从小公司来说，比如开智学堂，[用GitHub-wiki管理开智学堂学员、协作伙伴常用资料](https://github.com/OpenMindClub/Share/wiki)。国内的teambition虽然也有版本控制，但没有wiki功能，

### 如何使用GitHub建立简单的Blog

教程真的很多，对计算机语言不熟悉的童鞋，学习成本还是比较高的。如果只是作为版本控制，只需要建立file，没有必要建立Blog了。
那如果要建立Blog怎么做呢？（该教程不涉及编程，因为楼主不会 哭）

1. follow以下网址的每一步骤：https://pages.github.com/
   需要注意的是“What git client are you using?”，刚介绍了git是一套系统，需要运行在一个客户端，选择“I don't know”，网页会提示你下载什么客户端的。

1. jekyll安装
Jekyll 帮你轻松的搭建你的静态网页
[jekyll官网说明]（http://jekyll.com.cn/）
[jekyll环境安装]（http://jekyll.com.cn/docs/installation/）

1. 下载jekyll主题
http://jekyllthemes.org/
下载theme，解压的文件（不是文件夹，是文件夹下的子文件）复制到本地的网站根目录下，比如我的根目录：
C:\Users\Administrator\Documents\GitHub\username（你的用户名）.github.io

1. commit
打开GitHub桌面软件，切换到change目录下，可以看到刚刚复制的文件已经在change下显示，这时候commit to master就可以，点击同步，网页会同步更新
