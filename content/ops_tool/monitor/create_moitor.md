---
title: "创建监控告警"
description: 本小节主要介绍如何创建监控告警。
draft: false
weight: 1
---

## 功能描述

监控告警功能是基于虚拟资源层面的监控数据，针对平台中的时序数据进行监控，例如虚拟机的内存利用率、CPU 利用率等。平台目前支持的监控对象为虚拟机，支持用户自定义告警规则和监控周期，监控告警有助于用户及时了解资源使用情况和处理突发事件。


## 场景描述

该任务主要用于指导用户在云平台的运维工具中创建监控告警。

## 前提条件

已获得**云平台**的登录账户和密码。

## 操作步骤

1. 登录管理平台。

2. 在顶部导航栏，选择**运维工具** > **监控告警**，进入**监控告警**列表页面。

   ![create_monitor_1](../../_images/create_monitor_1.png)

3. 点击**创建监控告警**，在弹出的创建监控告警窗口中的**设置告警参数**页面，设置告警对象、监控周期以及告警规则，点击**下一步**。

   > **说明：**
   >
   > 云平台支持设置监控对象**满足任何一条告警规则便触发告警消息**或者**满足全部告警规则才触发告警信息**。具体方法可参考[设置告警状态触发条件](/ops_tool/monitor/manage_monitor#修改告警触发条件)相关内容。

   ![create_monitor_2](../../_images/create_monitor_2.png)

- **参数说明**
   
   <table>
   <tr>
   <th style="width:30%">参数</th>
   <th style="width:70%">详细说明</th>
   </tr>
   <tr>
    <td> 告警对象</td>
    <td> 目前仅支持对主机进行告警。</td>
   </tr>
   <tr>
    <td>监控周期</td>
    <td> 针对各项告警规则的监控周期，支持1分钟或5分钟。</td>
   </tr>
   <tr>
    <td>设置告警规则</td>
    <td>支持设置针对 CPU 利用率、内存利用率、磁盘使用量、硬盘 INONE、内网出流量、内网进流量的告警规则</td>
   </tr>
   </table>

4. 在创建监控告警窗口中的**设置告警方式**页面，设置各项参数，点击**创建**即可。

   ![create_monitor_3](../../_images/create_monitor_3.png)

- **参数说明**
   
   <table>
   <tr>
   <th style="width:30%">参数</th>
   <th style="width:70%">详细说明</th>
   </tr>
   <tr>
    <td> 告警名称</td>
    <td> 用户自定义，便于搜索与浏览。</td>
   </tr>
   <tr>
    <td>发送通知</td>
    <td> 是否发送告警通知，若选择是，则需配置发送条件、发送通知次数以及通知列表相关参数。</td>
   </tr>
   <tr>
    <td>满足以下条件发送通知</td>
    <td>可单独或全部勾选“资源发生警告时”、“资源恢复正常时”两种条件下发送告警通知。</td>
   </tr>
   <tr>
    <td>持续告警时，连续发送通知次数</td>
    <td>支持设置1 ～ 5次</td>
   </tr>
   <tr>
    <td>通知列表</td>
    <td>接收告警通知的邮箱列表。若无可选列表，需点击右侧<b>创建通知列表</b>进行创建。</td>
   </tr>
   </table>