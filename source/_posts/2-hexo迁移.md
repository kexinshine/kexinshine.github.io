---
title: 2-hexo迁移
date: 2021-06-18 20:48:28
tags: [git,hexo]
categories: [hexo]
---

# 多Git账号管理
## 配置ssh
```bash
ssh-keygen -t rsa -C "913178007@qq.com"
```
分别生成多个密钥例如id_rsa(公司git)，id_rsa_me(个人博客git)，并分别将.pub里的内容复制到各自的ssh里

## 配置config
```bash
vi ～/.ssh/config

#company
Host xxx.com
HostName xxx.com
User *@xxx.com
IdentityFile ~/.ssh/id_rsa

#blog
Host github.com
HostName github.com
User 913178007@qq.com
IdentityFile ~/.ssh/id_rsa_me
```
<!--more-->

# 安装hexo(mac系统)
## 安装node.js
[Node.js](https://nodejs.org/en/)

## 安装hexo
```bash
sudo npm install --unsafe-perm --verbose -g hexo
sudo npm install --unsafe-perm --verbose -g hexo-server
```





