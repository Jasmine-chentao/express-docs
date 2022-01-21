---
title: "实例规格"
description: Redis Standalone 提供的资源配置类型。
keyword: 资源配置,实例类型，,键值数据库,Redis,Redis Standalone,数据库
weight: 16
collapsible: false
draft: false
---



Redis Standalone 提供**预置资源规格**和**自定义资源规格**两种实例版本。

## 预置资源规格

Redis Standalone 提供 `多线程生产环境`、`单线程生产环境`、`多线程测试环境`、`单线程测试环境` 四种类型的资源配置，满足您不同场景下的业务需求。

> **说明**
> 
> -仅 Redis 6.x 版本提供预置资源配置。
> 
> -默认**存储磁盘类型**为 `企业型SSD本地盘`，磁盘存储容量可选 10～1000GB。

| 资源配置   | 云服务器 |  CPU       | 内存          | QPS 参考值 |
| :-------------- | :------------ | :------------- | :----------------- | :---------- |
| 多线程生产环境 | 通用型 e3    | 8（CPU 独享） | 8G，16G，32G，64G | 500000     |
| 单线程生产环境 | 通用型 e3    | 2（CPU 独享） | 4G，8G，16G       | 300000     |
| 多线程测试环境 | 基础型       | 8（CPU 共享） | 8G，16G，32G      | 150000     |
| 单线程测试环境 | 基础型       | 2（CPU 共享） | 2G，4G，8G        | 45000      |

## 自定义规格

> **说明**
> 
> -仅 Redis 5.x 版本支持自定义资源规格。
> 
> -默认**存储磁盘类型**为 `企业型SSD本地盘`，磁盘存储容量可选 10～1000GB。

| 云服务器 |  CPU       | 内存          | 
| :------------ | :------------- | :----------------- | 
| 通用型 e2    | 2核 | 1G、2G、4G，8G，16G、32G、64G       | 
| 基础型       | 1核 、2核| 1G、2G、4G，8G，16G、32G、64G       | 