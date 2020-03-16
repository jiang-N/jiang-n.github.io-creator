---
title: "使用Hugo搭建博客的记录"
date: 2020-03-15T10:47:54+08:00
draft: false
---

## Hugo简介
* Hugo是使用Go语言实现的一个博客生成器
* 是世界上最快的博客生成器

## 安装Hugo
[下载页面](https://github.com/gohugoio/hugo/releases)
1. 去下载页面下载hugo_xxx_Windows-64bit.zip
2. 解压，把hugo.exe存放到创建好的hugo目录下
3. 把上一步的路径添加到PATH中
4. 在终端输入**hugo version**如果看到一个版本号，说明安装成功
   ![查看是否安装成功](/static/images/20200316_01.jpg)
   
## 搭建博客
1. 在终端输入**hugo new site quickstart**创建一个新网站，quickstart可以替换成自己github的仓库名
   ![创建新站点](/static/images/20200316_02.jpg)
2. 添加一个主题，执行以下命令
   ![添加主题](/static/images/20200316_03.jpg)
3. 执行完上一步之后，接下来执行以下命令
   ![添加主题](/static/images/20200316_04.jpg)
4. 执行命令，创建你的第一篇博客
   ![添加主题](/static/images/20200316_05.jpg)
5. 开启Hugo服务器，执行以下命令
   ![添加主题](/static/images/20200316_06.jpg)

## 配置博客
1. 打开config.toml文件，可以对博客的标题、语言等选项进行配置
   ![配置博客](/static/images/20200316_07.jpg)
2. 生成静态页面，执行以下命令即可在本地生成一个public文件夹
   ![生成静态页面](/static/images/20200316_08.jpg)

## 更换主题
