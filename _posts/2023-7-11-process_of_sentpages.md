---
layout: post
title:  "使用git上传博客"
date:   2023-7-11 20:51:30 +0800--
categories: [部署]
tags: [YOLOv5]  
---


## 使用git链接github给本地建仓库
v5
首先下载安装git方法百度。  

新建作为仓库的文件夹，右键git bash here。  

## 1.打开git，在git命令窗口分别输入以下命令：  
    首先填写本地信息 
    $ git config --global user. name "github用户名"  
    $ git config --global user. email "github邮箱" 
    生成ssh密码  
    $ ssh-keygen -t rsa -C "githu邮箱"   
    然后分别打开：此电脑 —— 用户 —— .ssh   
    右键使用vscode打开.ssh文件里的id_rsa_pub文件,复制里面的密钥。  

## 2.回到github界面  
    点击右上角自己账号 —— settings —— SSH and GPG keys —— new SSH key   
    title：备注  
    key：密钥复制进去  
    点击add key    

## 3.找到仓库文件作为仓库的文件夹，右键git bash here。  
    $ ssh -T git@github.com 检测是否链接了github   
    github上传文件   
    git init   
    git add README . md    
    git commit -m "first commit"   
    第一次要加github仓库地址：   
    git remote add origin "仓库地址  
    例如：git@github.com:Temp. github-io.git"   
    //git branch -M main   
    git push -u origin master   //开始上传   

## 4.上传博客   
    $ git add. //推送全部更改  
    $ git commit -m "推送备注"  
    $ git push   //推送   

 

 





