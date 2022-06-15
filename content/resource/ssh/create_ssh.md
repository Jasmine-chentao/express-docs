---
title: "创建 SSH 密钥"
description: 本小节主要对云平台内资源页面中的存储进行介绍。
draft: false
weight: 1
---

## 功能描述

SSH 密钥可以为主机的 root 用户设置 SSH 公钥，当主机启动后，用户可使用 SSH 密钥进行 SSH 无密码登录。相对于用户名密码方式，密钥方式拥有更强的安全性，也可以很大程度阻止暴力破解的发生。目前常用的密钥都是非对称性的加密方式，主机内置公钥，而用户则拥有私钥。由于采用非对称加密，入侵者试图通过公钥去破解私钥难度会远远超出密码的破解。


## 场景描述

该任务主要用于指导用户在云平台内创建 SSH 密钥。

## 前提条件

已获得**云平台**的登录账户和密码。


## 操作步骤


1. 登录管理平台。

2. 在顶部导航栏，选择**资源** > **SSH 密钥**，默认进入 SSH 密钥列表页面。
 
   ![create_ssh_1](../../_images/create_ssh_1.png)

### 创建新密钥 

1. 点击**创建 SSH 密钥**，在弹出的创建密钥窗口中，创建方式选择**创建新密钥**，设置**密钥名称**，点击**创建**即可。

   ![create_ssh_2](../../_images/create_ssh_2.png)

2. 创建成功的新密钥会显示在 SSH 密钥列表中。在弹出的 **SSH 密钥已创建**的提示窗中，点击**下载**可将新密钥保存至本地。
    
    > **注意：**
    >
    > 平台不会保管用户的密钥，请在 10 分钟内点击“下载”按钮获取密钥

   ![create_ssh_3](../../_images/create_ssh_3.png)

### 使用已有公钥

1. 在 SSH 密钥列表页面，点击**创建 SSH 密钥**，在弹出的创建密钥窗口中，创建方式选择**使用已有公钥**，设置密钥**名称**，并将复制的公钥粘贴至相应的位置，点击**创建**即可。

   ![create_ssh_4](../../_images/create_ssh_4.png)

