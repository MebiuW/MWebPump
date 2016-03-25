# 动手写一个Python Web 框架学习笔记 - 搭建开发环境 （1）
#1 前言
很久以前，就一直想做一个网站，一来可以存一下在CSDN写的Leetcode记录，而来可以做一些自己想做的事情。
我在想用什么框架，如果用了PHP的话，我肯定会毫不犹豫的选择ThinkPHP+Wordpress，但是我又想趁机学下Python，Python看起来没有没有什么我特别喜欢的Web框架，然后正巧看到一篇动手写Python Web框架的教程，我想要不我就跟着做一下好吧，这里顺手也做一个Blog记录下。

[这个就是我看的教程，我很多可能都是基于他的来做的，所以可以去围观他的教程](http://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/001432170937506ecfb2f6adf8e4757939732f3e32b781c000)

#2 搭建开发环境
我个人对环境搭建不是很熟悉，总之先说下我的环境吧，OSX+Python3.4+MySQL，其他都没有，而这篇笔记也会基于这个基础开始，要是还没有的同学可以自行安装，我也不太会说怎么配置了。

##1 step 1 确认开发环境
首先请到你们的终端输入（应该Linux和OSX都能用这个命令，Windows的CMD或许也可以吧）

```
python -- version

```
确认环境是Python3.4.3
##2 step2 安装依赖环境
这里按照原博主的描述，使用pip安装一些Web所需要的第三方库：
异步框架aiohttp：
```
pip3 install aiohttp

```
前端模板引擎jinja2：
```
pip3 install jinja2

```
MySQL的Python异步驱动程序aiomysql：
```
pip3 install aiomysql

```

而MySQL数据库安装比较简单，这里就不表述了，记住自己的密码就好了。比如我自己喜欢直接装一个套件，或是用XAMPP也可以。

##3 step3 创建项目目录

随后根据原文的要求建立文档，我这里略微有点不太一样，寻找一个根目录建立如下的文件夹，剩下的文件或文件夹可以根据自己的需求增加
我只创建了我打星号的那一部分
```
awesome-python3-webapp/  <-- 根目录*
|
+- backup/               <-- 备份目录*
|
+- conf/                 <-- 配置文件*
|
+- dist/                 <-- 打包目录*
|
+- www/                  <-- Web目录，存放.py文件*
|  |
|  +- static/            <-- 存放静态文件*
|  |
|  +- templates/         <-- 存放模板文件*
|
+- ios/                  <-- 存放iOS App工程
|
+- LICENSE               <-- 代码LICENSE
```

##4 step4 使用Git
随后，这就是使用Git自己备份下了，没太多好说的




