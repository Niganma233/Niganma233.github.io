---
layout:       post
title:        "白嫖赛博大善人"
author:       "WHY"
header-style: text
catalog:      true
tags:
    - cloudflare
    - Web
---

> 在网上看到了个可以用赛博大善人部署的项目，所以更新一篇博客来记录一下。  

# 项目内容
共有两个项目，一个用来管理自己的计划可以推送到微信或电报  
另一个可以做影视聚合  

# 前期准备
1. Cloudflare 账号 <a href="https://cloudflare.com/" target="_blank" rel="noopener noreferrer">前往注册</a>
2. GitHub 账号 <a href="https://github.com/" target="_blank" rel="noopener noreferrer">前往注册</a>
3. 自己的域名(需托管到Cloudflare上，且若你有科学上网环境那么可以忽略) <a href="https://dash.domain.digitalplat.org/" target="_blank" rel="noopener noreferrer">前往获取</a>或自行购买

# 开始部署
## 先说第一个
1. 访问这个地址<a href="https://github.com/wangwangit/SubsTracker" target="_blank">项目一</a>打开index_v3.js并复制里面的代码。  
然后登录你的cloudflare创建worker，将代码粘贴进去并点击部署  
![粘贴代码](/img/subs.png)  
2. 创建KV键值 SUBSCRIPTIONS_KV  
![KV](/img/KV.png)  
3. 给worker绑定上键值对,以及设置定时执行时间!
![KV](/img/time.png)  
4. 打开worker提供的域名地址或你自己绑定的域名,输入默认账号密码: admin password (或者是：admin admin123),可以在代码中查看默认账号密码!  
让后你就可以自行配置你要发送给自己的提醒了。

## 第二个
1. 访问这个地址<a href="https://github.com/LibreSpark/LibreTV" target="_blank">LibreSpark/LibreTV: 一分钟搭建影视站</a>
2. fork一份到你自己名下
3. 在你的cloudflare Pages中创建项目并链接你fork的代码库
4. 在环境变量中设置PASSWORD和ADMINPASSWORD变量
5.　享受独属于你的影视聚合