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
那如果要建立Blog怎么做呢？（该教程不涉及编程，因为楼主不会:cry:）

1. follow以下网址的每一步骤：https://pages.github.com/
   需要注意的是“What git client are you using?”，刚介绍了git是一套系统，需要运行在一个客户端，选择“I don't know”，网页会提示你下载什么客户端的。

1. jekyll安装
Jekyll 帮你轻松的搭建你的静态网页
[jekyll官网说明](http://jekyll.com.cn/)
[jekyll环境安装](http://jekyll.com.cn/docs/installation/)

1. 下载jekyll主题
http://jekyllthemes.org/
下载theme，解压的文件（不是文件夹，是文件夹下的子文件）复制到本地的网站根目录下，比如我的根目录：
C:\Users\Administrator\Documents\GitHub\username（你的用户名）.github.io

1. commit
打开GitHub桌面软件，切换到change目录下，可以看到刚刚复制的文件已经在change下显示(有显示说明有修改)，这时候commit to master就可以（也就是同意改动），点击同步，网页会同步更新

### 配置jekyll theme

复制来的主题，通常是要修改的：
1. Blog名称，博客介绍，个人介绍，个人照片：在_config.yml中修改
2. 添加自己的文章：在_posts下添加，标题必须是英文的“year-month-day-title”。有些童鞋想要中文的title怎么办，是有代码的，我复制的Blog已经写好了，其它的模板不好说，楼主不懂代码:cry:
比如我的每篇文章开头就有以下代码，可以将title改为中文的。
```
layout: post
title: How to create GitHub page
date: 2017-10-26 17:00:00 +0300
```

[官方jekyll配置说明](https://help.github.com/articles/configuring-jekyll/)

[Adding Jekyll plugins to a GitHub Pages site](https://help.github.com/articles/adding-jekyll-plugins-to-a-github-pages-site/)


### 遇到的一些问题

1. 插入的图片在GitHub能显示，在jekyll上不能显示，在图片结尾增加"?raw=true"


>Provided that you have the image in your repo, you can use a relative URL:
>
>```![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")```
>
>If you need to embed an image that's hosted elsewhere, you can use a full URL
>
>```![Alt text](http://full/path/to/img.jpg "Optional title")```
>
>GitHub recommend that you use relative links with the ?raw=true parameter to ensure forked repos point correctly.
>
> 引用来源 https://stackoverflow.com/questions/10189356/how-to-add-screenshot-to-readmes-in-github-repository

2. 文章目录页引用文章内容的前几行

比如：

![thumbnail text](assets/markdown-img-paste-20171031130247102.png)

在index.html中注意以下引用的code，truncate是引用的字符个数，而truncatewords是引用的单词个数，大概是编码规则不一样，导致会有各种问题产生，当我设置到```turncate:200```的时候，就没什么问题了。

```{{post.content | strip_html | truncate:200}}```
