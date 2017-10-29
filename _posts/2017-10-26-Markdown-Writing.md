---
layout: post
title: 怎样用Markdown写作
date: 2017-10-26 21:00:00 +0300
description: Markdown是一种简单的语言，用它写作，就不用总想着用什么格式去修改。让写作回归写作的本质。 # Add post description (optional)
img: software.jpg # Add image post (optional)
tags: [Productivity] # add tag
---

先看三篇文章
1. 用 Markdown 写作的好处见  [Markdown写作浅谈](http://mp.weixin.qq.com/s/HsPZLl60vjbEKEbT2HHH7A)
2. Markdown 语法指南见  [Mastering Markdown · GitHub Guides](https://guides.github.com/features/mastering-markdown/)。
3. Atom是开源的，支持很多Markdown packages，可以扩展一些很赞的功能，Markdown的预览，以及插入图片，看这篇文章就知道啦：[使用Atom打造无懈可击的Markdown编辑器](http://www.cnblogs.com/libin-1/p/6638165.html)。

你要是这三篇都看完，那Markdown的使用就基本没有问题了。

另外值得注意的是，GitHub的Guides中没有提到 'color', 'css', 'html', or 'style'，因此用这些写的无法在GitHub上显示；下面的举例中，也会明确指出哪些适用于GitHub，哪些不适用。

## emoji(适用于GitHub)

  如果是GitHub写作，只要调用“：”就可以了。在Atom里，要添加一个package—[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)，输入“:s”，就可以调用了:smiley:

有哪些emoji可以用呢？来看看[小抄表](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

## 表格(适用于GitHub)
  **Markdown写法**

  ![table](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026113646668.png)

  **Markdown呈现样式**

  软件|Atom  |简书  |为知
  -|-----|  ----| ----|
  功能|编辑|写作 |知识管理

## Highlight(适用于GitHub，但Atom中无法显示)

![Highlight](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026133106904.png)

```diff
+ 加号代表highlight绿色
- 减号代表highlight红色
```

## 字体(不适用于GitHub)

  **Markdown写法**

![font](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-2017102612053162.png)

  **Markdown呈现样式**

  1. <font face="黑体">我是黑体</font>
  1. <font face="微软雅黑">我是微软雅黑</font>
  1. <font color=#FF0000 face="宋体">我是红色宋体</font>
  1. <font color=gray size=5>我是灰色</font>

  另外颜色可以在这个网站查询[RGB颜色参考](http://tool.oschina.net/commons?type=3)

## 底色/背景色(不适用于GitHub)

  **Markdown写法**

![背景色](https://github.com/Marina-Ma/Marina-Ma.github.io/blob/master/assets/img/markdown-img-paste-20171026125110889.png)

  **Markdown呈现样式**
  <table><tr><td bgcolor=#0e88e3>这里的背景色是#0e88e3</td></tr></table>

  配色参考[Color Palettes Color Schemes](http://www.color-hex.com/color-palettes/)

*该帖不定期更新*
