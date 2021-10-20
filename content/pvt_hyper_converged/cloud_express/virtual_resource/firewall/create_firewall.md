---
title: "创建防火墙"
description: 本小节主要介绍青立方® 超融合易捷版 防火墙。 
keywords: 青立方® 超融合易捷版，创建防火墙
weight: 10
collapsible: false
draft: false
---


防火墙规则可定义允许或阻止的互联网流量类型。

初始状态下，每个防火墙都不包含任何规则，即任何端口都是封闭的，需要建立规则以打开相应的端口。

> **注意**
>
> 开放外网端口存在一定风险，如 Windows 3389、Redis 6379、Elasticsearch 9300、数据库 3306 等被攻击风险较高的端口。若开放 ssh 22 端口，请您确保禁用密码登录，使用密钥方式登录。

## 创建防火墙

1. 登录 青立方® 超融合易捷版。
2. 选择 **虚拟资源** > **安全**，进入安全管理列表。

   ![防火墙列表](../../../_images/firewall_list.png)

3. 点击 **+ 创建防火墙**，弹出防火墙配置窗口。
4. 配置防火墙的基本信息。

   配置防火墙名称，示例名称为 `demo_firewall`。

5. 点击**确认**，继续配置防火墙规则。

   防火墙规则添加支持快捷方式，如在右侧快速配置 ping、ssh、http 等规则。

    -规则名称：为防火墙起一个简洁明了的名称，便于用户浏览和搜索。
    
    -优先级：防火墙规则的优先级决定规则应用至网络流量的顺序，数字越小优先级越高。
    
    -规则：**下行规则**可控制 Internet 用户对服务器的访问规则（如仅向用户开放网站访问）；**上行规则**可控制服务器可访问的 Internet 访问(如让服务器仅能访问微信 API)，从而全面的保护业务安全。
    
    -协议：支持多协议设置，如常用的 TCP、UDP。
    
    -起始端口：1~65525，可点击右侧标志，选择已创建的 IP /端口集合。
    
    -结束端口：1~65525。
    
    -源 IP：不填表示所有 IP 地址，可点击右侧标志，选择已创建的 IP/端口集合。

   ![配置防火墙](../../../_images/config_firewall.png)

6. 确认配置信息无误后，点击 **确定**，返回防火墙列表页面。

以上示例在防火墙规则中，为 TCP 协议的 80 端口添加一条下行规则，命名为 firewall-demo，行为选择接受。Internet 用户可访问 80 端口的服务，外部流量能够正常通过该端口。

## 生效防火墙

新建或修改防火墙规则后，注意都需要应用修改。

1. 选择目标防火墙，点击防火墙 ID，进入防火墙详情页面。
2. 点击**应用修改**，保存并生效当前防火墙配置。

   ![生效防火墙](../../../_images/enable_firewall.png)