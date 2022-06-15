---
title: "创建定时器"
description: 本小节主要介绍如何创建定时器。
draft: false
weight: 1
---

## 功能描述

定时器功能可用来周期性地执行一系列的资源操作任务，比如根据业务需要定时开关主机、创建主机和创建备份等。可在指定的周期重复执行，也可仅执行一次，且每个任务支持多个资源批量操作。任务执行后会发出通知到用户指定的通知列表并保留近期执行的历史记录。

目前支持的定时任务包括：

- 关闭主机；
- 开启主机；
- 重启主机；
- 创建备份（硬盘、主机）；
- 启用安全组规则；
- 禁用安全组规则。


## 场景描述

该任务主要用于指导用户在云平台的运维工具中创建定时器。

## 前提条件

已获得**云平台**的登录账户和密码。

## 操作步骤

1. 登录管理平台。

2. 在顶部导航栏，选择**运维工具** > **定时器**，进入**定时器**列表页面。

   ![create_timer_1](../../_images/create_timer_1.png)

3. 点击**创建定时器**，在弹出的创建定时器的窗口中，设置定时器的基本信息参数，点击**创建**。

   ![create_timer_2](../../_images/create_timer_2.png)

- **参数说明**
   
   <table>
   <tr>
   <th style="width:30%">参数</th>
   <th style="width:70%">详细说明</th>
   </tr>
   <tr>
    <td> 名称</td>
    <td> 用户自定义，便于搜索与浏览。</td>
   </tr>
   <tr>
    <td>发送通知</td>
    <td>支持重复执行或仅执行一次。</td>
   </tr>
   <tr>
    <td>周期</td>
    <td>支持每天、每 N 天、每 N 小时、每周、每月。</td>
   </tr>
   <tr>
    <td>时间</td>
    <td> 设置定时器的执行时间。</td>
   </tr>
   <tr>
    <td> 推送条件</td>
    <td> 可根据执行状态推送至消息中心。</td>
   </tr>
   </table>

4. 在定时器创建后，在**创建定时器**窗跳转至**添加定时任务**页面，设置相关定时任务参数后，点击**添加**即可。

   ![create_timer_3](../../_images/create_timer_3.png)

- **参数说明**
   
   <table>
   <tr>
   <th style="width:30%">参数</th>
   <th style="width:70%">详细说明</th>
   </tr>
   <tr>
    <td> 名称</td>
    <td> 用户自定义，便于搜索与浏览。</td>
   </tr>
   <tr>
    <td>执行操作</td>
    <td>支持开启主机、关闭主机、重启主机、创建备份、启用安全组规则、禁用安全组规则。</td>
   </tr>
   <tr>
    <td>选择操作对象</td>
    <td>针对执行操作的不同，对象可能是虚拟主机、硬盘或安全组规则。</td>
   </tr>
   </table>


5. 定时任务创建完成后，返回定时器列表新创建的定时器显示在列，点击定时器名称，进入其详情页面，可查看当前定时任务状态为`已启用`。

   ![create_timer_4](../../_images/create_timer_4.png)


