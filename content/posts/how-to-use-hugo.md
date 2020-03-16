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
   ```
   hugo version
   ```
   

## 搭建博客
1. 在终端输入**hugo new site quickstart**创建一个新网站，quickstart可以替换成自己github的仓库名
   ```
   hugo new site quickstart
   ```
   
2. 执行以下命令添加一个主题
   ```
   cd quickstart
   git init
   git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
   ```

3. 执行完上一步后执行命令
   ```
   echo 'theme = "ananke"' >> config.toml
   ```

4. 执行命令，创建你的第一篇博客
   ```
   hugo new posts/my-first-post.md
   ```

5. 执行以下命令来开启Hugo服务器
   ```
   hugo server -D
   ```


## 配置博客
1. 打开config.toml文件，可以对博客的标题、语言等选项进行配置
   ![配置博客](https://s1.ax1x.com/2020/03/17/8tKNnO.jpg)

2. 生成静态页面，执行以下命令即可在本地生成一个public文件夹
   ```
   hugo -D
   ```


## 更换主题
[更换主题地址](https://themes.gohugo.io/)

1. 进入上方网址，选择自己喜欢的主题进入主题详情页面，点击homepage按钮
   ![homepage按钮](https://s1.ax1x.com/2020/03/17/8tlo8A.png)

2. 在跳转过后的页面找到安装方法

3. 在config文件中更改对应的主题名即可