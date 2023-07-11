---
layout: post
title:  "使用git上传博客"
date:   2023-7-11 20:51:30 +0800--
categories: [部署]
tags: [installation, blog, setting up]  
---


# 使用git链接github给本地建仓库

首先下载安装git方法百度。  

新建作为仓库的文件夹，右键git bash here。  

## 1.打开git，在git命令窗口分别输入以下命令：  <br>
    首先填写本地信息  <br>
    $ git config --global user. name "github用户名"  <br>
    $ git config --global user. email "github邮箱" <br>
    生成ssh密码   <br>
    $ ssh-keygen -t rsa -C "githu邮箱"   <br>
    然后分别打开：此电脑 —— 用户 —— .ssh   <br>
    右键使用vscode打开.ssh文件里的id_rsa_pub文件,复制里面的密钥。  <br><br>
## 2.回到github界面  <br>
    点击右上角自己账号 —— settings —— SSH and GPG keys —— new SSH key   <br>
    title：备注  <br>
    key：密钥复制进去  <br>
    点击add key    <br>
## 3.找到仓库文件作为仓库的文件夹，右键git bash here。   <br>
    $ ssh -T git@github.com 检测是否链接了github    <br>
    github上传文件   <br>
    git init   <br>
    git add README . md    <br>
    git commit -m "first commit"   <br>
    第一次要加github仓库地址：   <br>
    git remote add origin "仓库地址，例如：git@github.com:Temp. github-io.git"  <br>
    //git branch -M main   <br>
    git push -u origin master   //开始上传   <br>
## 4.上传博客   
    $ git add. //推送全部更改  <br>
    $ git commit -m "推送备注"  <br>
    $ git push   //推送   <br>

 
 



regards.
<h4 align = "right">oukohou.</h4>

