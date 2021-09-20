---
title: 安装须知
keywords: 
last_updated: 2021-9-8
# tags: [getting_started]
summary: 在安装之前请先阅读该须知。
topnav: topnav_zh
sidebar: v1_zh_sidebar
permalink: v1_zh_install_instruction.html
folder: v1_zh
---

## 支持平台

目前，Vocab Manager 1.x 仅支持 Windows 平台，其它平台的用户可能需要寻找相应平台的相似产品作为替代。


## 安装和使用

推荐安装在侧边栏 “Windows” 中的最新版本进行下载。

按安装时，需要为软件指定一个文件夹，用于存放软件本身，以及用户的所有生词数据。

* **如果你希望在卸载/更新应用之前保留您的数据，你需要手动的拷贝安装目录下的 “LocalDB.sqlite” 文件进行备份。**

SQLite 为软件提供本地存储服务，这需要使用者具有对相关文件夹的读写权限。

* 如果您在使用软件时遇到 “attempt to write a read-only database” 的错误弹窗，请尝试退出程序，使用右键菜单中的 “以管理员身份运行” 选项重新打开软件。

## 版本与特性

主要版本 Vocab Manger 1.x 有多个内部版本，他们以递增的方式进行编号，如 1.0.0, 1.1.0, 1.2.0, ... 其中第二个数字表示新功能更新，第三个数字表示错误修复。

所有内部版本的安装包都在侧边栏 “Windows” 中，每个安装包的跟新都会有详细的错误修复、新特性相关信息。

**目前尚不支持自动更新和覆盖，用户在进行版本升级时，需要先手动进行数据备份，然后手动卸载旧版本、安装新版本，并将数据在新版本内进行覆盖。**