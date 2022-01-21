---
title: "基本概念"
description: 本小节主要介绍 Redis Standalone 基本概念。 
keyword: 基本概念,键值数据库,Redis,Redis Standalone,数据库
weight: 100
collapsible: false
draft: false
---




## Redis

Redis 是一种支持键值（Key-Value ）等多种数据结构的内存数据库。Redis 数据库使用 ANSI C 语言编写，提供字符串、哈希、列表、队列、集合结构直接存取。可用于缓存、事件发布或订阅、高速队列等场景。

有关 Redis 的详细介绍，请访问 [Redis 官方网站](https://redis.io/)。

## 用户管理 ACL

ACL 即访问控制列表（Access Control List），包含了对一个对象或一条记录可进行何种操作的权限定义。

**ACL 用户**即具备一定 ACL 规则的用户帐号。该用户帐号 ACL 权限是通过配置用户帐号允许获禁用 ACL 规则划定。

ACL 规则即权限控制字符串，用于给用户设置命令权限及数据权限，避免用户的误操作导致数据丢失或避免数据泄露的安全风险。

## 多可用区部署

将集群节点部署在不同的可用区域内，节点间物理隔离。您可以将应用程序也进行 多可用区部署，从而达到数据与应用全部高可用。

## 集群（Cluster）

一个 Redis Standalone 集群由一个或多个节点组成，并提供集群内所有节点资源的联合管理能力。

创建集群时系统随机分配通用唯一标识符（UUID）全局唯一，不可修改。同时一个集群的调用，由 ID 标识。您可以自定义一个集群的名称，以及为集群绑定标签，方便集群分组管理。

## 节点（Node）

一个节点是集群中的一个服务器，用来存储数据并参与集群的索引和搜索。节点的调用，由一个 ID 标识。您也可以自定义任意节点的名称，节点名称对于管理工作很重要。

一个集群可以创建多个节点。