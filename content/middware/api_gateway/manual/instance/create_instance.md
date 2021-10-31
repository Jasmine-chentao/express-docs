---
title: "创建专享实例"
linkTitle: "创建专享实例"
date: 2021-05-18T10:08:56+09:00
description:
draft: false
weight: 10
---

通过青云QingCloud 云平台 API 网关服务，您可以快速创建 API 网关专享实例。

本小节主要介绍如何快速创建 API 网关专享实例。



## 操作步骤

按照以下操作，创建 API 网关专享实例。

1. 登录 [QingCloud 管理控制台](https://console.qingcloud.com/login)。

2. 在控制台导航栏中，选择**产品与服务** > **消息队列与中间件** > **API 网关** ，进入**API 网关**页面。

3. 点击**实例管理** > **创建专享实例**，进入实例创建页面。

4. 填写实例购买信息。

   **实例计费模式**：支持『预留合约』与『按需付费』两种计费方式。

   > **说明**
   >
   > 『预留合约』模式，支付费用后用户在选择的时长内无需再支付其他实例费用，可选择是否自动续费，若账户余额充足到期自动扣费。
   >
   > 『按需付费』模式，以小时为单位计费。

   **区域及可用区**：建议根据您的业务区域选择临近区域，以减少网络时延，提高访问速度。另外，不同区域的资源价格可能有差异，您可以根据价格选择合适的区域。

5. 配置实例规格。

   QingCloud API 网关服务提供`基础版`、`专业版`、`企业版`、`企业高级版`、`企业铂金版`、`企业钻石版`六种专享实例规格。不同版本的最大请求数、SLA、最大连接数以及费用都不同，配置越高，费用越高。

6. 配置实例信息。

   ![create_apig2](../_images/create_apig2.png)

   **网络**：支持选择基础网络和 VPC 网络。若未创建 VPC 网络，请参考：[创建 VPC 网络](/../../../../network/vpc/manual/vpcnet/10_create_vpc/)。

   **带宽计费**：提供带宽计费（预付费模式，按小时收取费用），流量计费（后付费模式，用多少扣多少），且可设置带宽值，不同的带宽费用不同。

   **自动续费**：当用户选择预留合约时，在页面底部会显示勾选框是否自动续费，当前提供 1-11 个月，1-3 年的选项。勾选后在实例时长到期后若余额充足，根据勾选的自动续费时间，自动延期续费使用实例。

   ![create_apig3](../_images/create_apig3.png)	

   **时长**：针对预留合约的专享实例，用户可修改购买时长。不同时长有不同的折扣，时长越长折扣越大。

7. 点击立即购买，即可创建实例。创建时间约 5-10 分钟，请耐心等待。

   