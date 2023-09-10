---
title: tauri-notes-1
categories:
  - 学习
tags:
  - tauri
date: 2023-09-10 13:50:33
---

## 使用Tauri的准备

首先要配置好nodejs和npm环境，因为用的是arm linux，所以过程中踩了不少奇奇怪怪的坑，但好在基本都解决了：）

之后我用npm安装了pnpm，以后也pnpm做tauri项目的包管理器了。

使用pnpm安装完tauri和rust后，创建项目，我遇到了第一个坑。

## 使用过程中的第一个坑

创建完项目后，使用`pnpm tauri dev`开始构建应用，期间不断报错，像`Package 'gdk-3.0', required by 'virtual:world', not found`这种，解决方式捣鼓了很久，最后发现只要按照提示的内容安装对应的`lib...-x.x-dev`包就可以了。

之后再使用`pnpm tauri dev`就能成功出现窗口了。
