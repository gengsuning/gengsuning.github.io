---
layout: post
title: 如何使用百度统计监测网站流量
date: 2017-11-08
categories: blog
tags: 百度统计  
description: 文明的未来
---

前段时间使用GitHub Pages和Jekyll组件构造了自己的私人博客网站 [gengsuning.com](http://gengsuning.com) 。

新生事物，又没有经过推广，访问量可想而知是非常的少。但是到底有少到什么程度呢，我却一点概念都没有。

于是意识到这个博客还缺一个网站访问量的统计工具。

查了一些资料，发现百度系列的产品百度统计就可以干这个事，还挺方便的。算是为数不多的好产品。

以下就是使用百度统计监测自有网站流量的步骤：

-    首先需要注册百度统计的账号。注意这个账号不是普通的百度账号，而是百度推广的账号，总之可以先用普通的百度账号试一下，如果不行就重新注册一个，非常方便。

-    注册账号并登录进百度统计系统后，页面会自动跳转到获取代码页，有一个获取代码的醒目按钮，点击后获得以下一段代码：
>     <script>
>     var _hmt = _hmt || [];
>     (function() {
>         var hm = document.createElement("script");
>         hm.src = "https://hm.baidu.com/hm.js?xxxxxxxxxxxxxxxx";;
>         var s = document.getElementsByTagName("script")[0];
>         s.parentNode.insertBefore(hm, s);
>     })();
>     </script>

-    将这段代码拷到网站首页的<head>标签之前，或者将这段代码存为html文件，并在include文件中包含这个html文件即可.（注意代码中的xxxxxxxxxx实际是个人账号生成的key值，每个账号不同）

-  访问百度统计，可以查看各种维度统计的网站访问量图表。

通过百度统计的图表，对博客访问量，尤其是每一页的访问量，访客来源是什么等关键信息有了非常清晰的认识，对于提高网站质量也有大有裨益的事情。
