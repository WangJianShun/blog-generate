---
title: 论菜鸟是如何搭建他的Hexo博客
date: 2018-03-05 13:46:40
tags:
---
最近几天一直在跟着教程的指引开始做自己的hexo博客，中间遇到了许许多多的坑，还好在摸索当中渐渐找到了头绪，当然也仅仅是能够把基本的步骤完成的程度。我还需要更多的了解搭建hexo相关的知识。

下面就简单介绍一下根据我的学习所进行的操作
在github搭建博客系统可以分为以下几步：
## 搭建步骤
* ### 系统配置
* ### 安装Hexo
* ### 执行操作指令
* ### 编辑博客

### 系统配置
首先，我们要在gitHub上创建一个repo，repo名称的格式是[用户名.github.io]，（注意这个repo的命名格式，必须是你的用户名+github.io,错一点也不行）
### 安装hexo
在git bash上输入命令 npm install -g hexo-cli 开始下载hexo
### 执行操作指令
hexo init myBlog

cd myBlog

npm i

依次在git bash上输入

### 编辑博客
1. hexo new 标题，这里的标题替换成你想添加的内容，回车，命令行会出现一个刚刚生成的文件路径，window用户要把路径中的\ 改为/

2. 输入命令 start xxxxxxxxxxxx.md ,就可以打开编辑器，在里面输入你想编写的内容。

3. 输入命令start _config.yml 打开文件编辑网站配置，

4. 把第 6 行的 title 改成你想要的名字

5. 把第 9 行的 author 改成你的大名

6. 把最后一行的 type 改成 type: git

7. 在最后一行后面新增一行，左边与 type 平齐，加上一行 repo: 仓库地址 （请将仓库地址改为「你的用户名.github.io」对应的仓库地址，仓库地址以 git@github.com: 

8. npm install hexo-deployer-git --save，安装 git 部署插件

9. hexo deploy

10. 完成这些步骤，打开github page功能，打开链接就可以预览你的博客了~

往后再写新的博客的时候，只需要执行

hexo new 新的博客

start 路径 在里面编辑内容

hexo generate

hexo deploy

就可以发布一篇新的博客了。


