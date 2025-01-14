# 处理消息

## 视频示例

## 概述

对云扩 RPA 控制台（企业版）的“数据中心 > 数据队列”中的消息进行处理。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **部门**：选择控制台中的“数据队列”所在的部门。
- **数据队列**：选择需要处理消息的数据队列。

### 输出

- **消息**：获取到的队列数据，仅支持变量。

### 可选项

- **处理完成后**：消息处理完成后的行为。
- **无消息时**：当队列中没有消息时的行为。
- **监听等待时间**：无消息时，监听等待的时间。
- **时间单位**：与“监听等待时间”相对应的时间单位。

## 使用示例

**前置必要条件**：在企业版控制台的“数据中心 > 数据队列”中已创建数据队列。
**此流程执行逻辑**：从企业版控制台的“数据中心 > 数据队列”中，处理指定 `产品设计与测试组` 部门中的指定 `wx` 队列中的消息，处理完成后从队列中移除。

![设置处理消息](https://docimages.blob.core.chinacloudapi.cn/images/Activities/handlemessage20211122.png)
