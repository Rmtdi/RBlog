---
title: termux-proot-start-problem
categories:
  - 问题与解决
tags:
  - proot
date: 2024-01-18 08:02:03
---

## 问题

termux-proot的xfce桌面无法启动

## 分析

网上都是将termux和proot-linux的DISPLAY环境变量设为:0，不知为何它在我这儿不起作用，于是查阅了很久，最终在b站专栏一篇不引人注目的文章中找到解决方法。

## 解决

解决方法忘了，总的来说，就是把显示端口从:0改成:1，之后问题就迎刃而解了。

## 参考