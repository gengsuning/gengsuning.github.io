---
layout: post
title: 在国内如何访问StackOverFlow网站
date: 2017-10-29
categories: blog
tags: StackOverFlow FireFox
description: 小窍门
---

搞计算机的人都知道，StackOverFlow是全球最大的技术类问答网站，不过是英文的。国内有类似的技术类问答网站segmentfault.com,但是在活跃度和问题、回答的质量上显然不及前者。

但是在国内访问StackOverFlow有个问题，就是系统响应时间非常的慢，还经常超时无法显示页面。这是怎么回事呢？

原来，这个跟StackOverFlow调用的第三方服务有关，StackOverFlow会调用Google的JS服务，而由于Google在中国被墙，连带造成StackOverFlow也中招。

那么，有什么办法可以解决这个问题呢？方法是有的：

	1. 放弃使用360、chrome、IE等浏览器。
	2. 使用firefox浏览器，并安装Decentraleyes这个扩展插件。这个插件的作用就是在程序调用了不可用的服务时，可以提前中断调用。

经实际测试，这个方法非常靠谱。
