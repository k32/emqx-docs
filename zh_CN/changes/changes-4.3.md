---
# 编写日期
date: 2020-02-07 17:15:26
# 作者 Github 名称
author: wivwiv
# 关键字
keywords:
# 描述
description:
# 分类
category:
# 引用
ref:
---

# 版本发布

## 4.3-rc.4 版本

*发布日期: 2021-04-16*

EMQ X 4.3-rc.4 现已发布，主要包含以下改动:

### emqx

**功能增强:**

- Redis 哨兵模式支持 SSL 连接

  Github PR: [emqx#4553](https://github.com/emqx/emqx/pull/4553)

- WebSocket 连接支持获取真实 IP 与 Port

  Github PR: [emqx#4558](https://github.com/emqx/emqx/pull/4558)

- Prometheus 支持集群指标

  Github Issue: [emqx#4548](https://github.com/emqx/emqx/pull/4548)
  Github PR: [emqx#4572](https://github.com/emqx/emqx/pull/4572)

**错误修复:**

- 修复 MQTT 桥接飞行窗口的问题

  Github Issue: [emqx#3629](https://github.com/emqx/emqx/issues/3629)
  Github PR: [emqx#4513](https://github.com/emqx/emqx/pull/4513), [emqx#4526](https://github.com/emqx/emqx/pull/4526)
  
- 修复多语言扩展钩子无法处理返回的 false 值的问题

  Github PR: [emqx#4542](https://github.com/emqx/emqx/pull/4542)

- 默认启动模块，避免集群后内置模块无法正常工作

  Github PR: [emqx#4547](https://github.com/emqx/emqx/pull/4547)

- 修复认证数据无法导入的问题

  Github PR: [emqx#4582](https://github.com/emqx/emqx/pull/4582), [emqx#4528](https://github.com/emqx/emqx/pull/4528)

- 修复 WebSocket 连接无法使用对端证书作为用户名的问题

  Github PR: [emqx#4563](https://github.com/emqx/emqx/pull/4563)

- 修复 MQTT-SN 网关在睡眠模式下会丢弃 DISCONNECT 报文的问题

  Github Issue: [emqx#4506](https://github.com/emqx/emqx/issues/4506)
  Github PR: [emqx#4515](https://github.com/emqx/emqx/pull/4515)

- 修复 LwM2M 网关将数字编码、解码为无符号整型的问题

  Github Issue: [emqx#4499](https://github.com/emqx/emqx/issues/4499)
  Github PR: [emqx#4500](https://github.com/emqx/emqx/pull/4500)

- 修复部分 HTTP API 不可用的问题

  Github Issue: [emqx#4472](https://github.com/emqx/emqx/issues/4472)
  Github PR: [emqx#4503](https://github.com/emqx/emqx/pull/4503)

## 4.3-rc.3 版本

*发布日期: 2021-03-30*

EMQ X 4.3-rc.3 现已发布，主要包含以下改动:

### emqx

**错误修复:**

- 限制飞行窗口的最大长度为 65535

  Github PR: [emqx#4436](https://github.com/emqx/emqx/pull/4436)

- 修复 Server Keep Alive 生效情况下 Dashboard 中 Keep Alive 字段的值未同步的问题

  Github PR: [emqx#4444](https://github.com/emqx/emqx/pull/4444)

- OOM 时快速杀死连接进程

  Github PR: [emqx#4451](https://github.com/emqx/emqx/pull/4451)

- 修复 `emqx start` 报超时但服务实际已启动的问题

  Github PR: [emqx#4449](https://github.com/emqx/emqx/pull/4449)

- 修复 MQTT-SN 睡眠模式不可用的问题

  Github PR: [emqx#4435](https://github.com/emqx/emqx/pull/4435)

## 4.3-rc.2 版本

*发布日期: 2021-03-26*

EMQ X 4.3-rc.2 现已发布，主要包含以下改动:

### emqx

**错误修复:**

- 修复 emqx 和 emqx_ctl 命令在某些情况下不可用的问题

  Github PR: [emqx#4430](https://github.com/emqx/emqx/pull/4430)

## 4.3-rc.1 版本

*发布日期: 2021-03-23*

EMQ X 4.3-rc.1 现已发布，主要包含以下改动:

### emqx

**功能增强:**

- 支持 observer_cli

  Github PR: [emqx#4323](https://github.com/emqx/emqx/pull/4323)

- 支持清除所有 ACL 缓存

  Github PR: [emqx#4361](https://github.com/emqx/emqx/pull/4361)

- SSL 支持 `verify` 与 `server_name_indication` 配置项

  Github PR: [emqx#4349](https://github.com/emqx/emqx/pull/4349)

**错误修复:**

- 修复主题重写与 ACL 执行顺序导致的问题

  Github Issue: [emqx#4200](https://github.com/emqx/emqx/issues/4200)
  Github PR: [emqx#4331](https://github.com/emqx/emqx/pull/4331)

- 修复 MQTT 报文接收计数问题

  Github PR: [emqx#4371](https://github.com/emqx/emqx/pull/4371)

- 修复心跳报文的处理

  Github Issue: [emqx#4370](https://github.com/emqx/emqx/issues/4370)
  Github PR: [emqx#4371](https://github.com/emqx/emqx/pull/4371)

- 修复由于默认的 SSL Ciphers 中包含了 OTP 22 不支持的 Ciphers 导致使用 OTP 22 编译后启动失败的问题

  Github PR: [emqx#4377](https://github.com/emqx/emqx/pull/4377)

## 4.3-beta.1 版本

*发布日期: 2021-03-03*

EMQ X 4.3-beta.1 现已发布，主要包含以下改动:

### emqx

**功能增强:**

- 减少开启规则引擎插件时的性能损耗

  Github PR: [emqx#4160](https://github.com/emqx/emqx/pull/4160)

- 仅在正式版本中启用数据遥测功能

  Github PR: [emqx#4163](https://github.com/emqx/emqx/pull/4163)

- 支持重启监听器

  Github PR: [emqx#4188](https://github.com/emqx/emqx/pull/4188), [emqx#4190](https://github.com/emqx/emqx/pull/4190)

- 禁用规则的同时销毁动作占用的资源

  Github PR: [emqx#4232](https://github.com/emqx/emqx/pull/4232)

- 共享订阅分发策略配置为 `round_robin` 时随机选择起始点

  Github PR: [emqx#4232](https://github.com/emqx/emqx/pull/4232)

- 允许使用 Base64 编码的客户端证书或者客户端证书的 MD5 值作为用户名或者 Client ID

  Github PR: [emqx#4194](https://github.com/emqx/emqx/pull/4194)

- 保持对 EMQ X Broker 启动后连接失败的资源进行重试

  Github PR: [emqx#4125](https://github.com/emqx/emqx/pull/4125)

**错误修复:**

- 修复过长的 Client ID 无法追踪的问题

  Github PR: [emqx#4163](https://github.com/emqx/emqx/pull/4163)

- 修复查询客户端信息可能出现崩溃的问题

  Github PR: [emqx#4124](https://github.com/emqx/emqx/pull/4124)

## 4.3-alpha.1 版本

*发布日期: 2021-01-29*

EMQ X 4.3-alpha.1 现已发布，主要包含以下改动:

*功能*

- 支持 Erlang/OTP 23
- 新安装包仅支持 macOS 10.14 及以上版本
- 规则引擎新增更新资源逻辑
- 增强 Webhook 与 HTTP 认证性能
- 多语言扩展功能底层实现方式由 erlport 改为 gRPC
- 保护 EMQ X Broker 免受跨站点 WebSocket 劫持攻击
- 项目调整为 umbrella 结构
- 解决集群环境下节点必须按首次启动顺序启动，否则需要等待前置节点启动的问题
- Websocket 监听器支持从 subprotocols 列表中选择支持的 subprotocol
- 支持 MySQL 8.0 的默认认证方法 caching_sha2_password
- JWT 认证支持 JWKS
- 支持配置证书链最大长度以及私钥文件密码
- 支持 Mnesia 认证信息的导入导出
- 共享订阅支持按源主题的 Hash 分发消息

*BUG*

- 修复 ekka_locker 在极端条件下内存可能无限增长的问题
- 修复 MQTT 桥接功能中 `max_inflight_size` 配置项不生效的问题
- 修复 CoAP 连接中 ACL 配置不生效的问题
- 修复使用相同 ClientID 的 CoAP 客户端可以同时接入的问题
- 修复告警持续时间计算错误的问题
- 修复 MySQL 认证 SSL/TLS 连接功能不可用的问题
- 修复 MQTT 桥接功能中指标统计错误和 `retry_interval` 字段进行了多次单位转换的问题
- 修复 Redis 重连失败问题
