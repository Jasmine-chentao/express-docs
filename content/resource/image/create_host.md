---
title: "基于镜像创建主机"
description: 本小节主要介绍基于镜像创建主机的具体操作流程。
draft: false
weight: 2
---

## 功能描述

主机是以虚拟机的形式运行在云平台中的镜像副本。基于一个镜像，用户可以创建任意数量的主机。在创建主机时，用户需要指明 CPU、内存和系统盘等配置。


## 场景描述

该任务主要用于指导用户在云平台内基于镜像创建主机。

## 前提条件

- 已获得**云平台**的登录账户和密码。
- 云平台内已存在可用镜像。

## 操作步骤

1. 登录管理平台。

2. 在顶部导航栏，选择**资源** > **镜像**，进入镜像列表页面。

3. 点击指定镜像所在行的更多操作<img src="../../_images/more_operation.png" style="zoom:50%;" />，选择**基于镜像创建主机**，

   > **注意：**
   >
   > 基于镜像创建之前，需要先注册用户上传的本地镜像，或者预先将主机制作成镜像。

   ![create_host_1](../../_images/create_host_1.png)


4. 在弹出**创建新虚拟主机**的页面，填写待创建虚拟机的基本信息，支持自定义虚拟机配置，可参考[创建 ExpressCloud 主机](/resource/virtual/expresscloud/create_virtual)相关内容。

   ![create_host_2](../../_images/create_host_2.png)

5. 完成基本信息配置后，点击**创建**即可基于当前镜像创建新的虚拟机。

