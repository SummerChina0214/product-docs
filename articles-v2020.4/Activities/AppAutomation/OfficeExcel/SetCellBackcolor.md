# 设置单元格背景色

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/SetCellsbackground.mp4"></video>

## 概述

对指定单元格进行填充背景色(16 进制颜色码)操作。

> **说明：**
>
> 该组件需在 Office Excel 的 **打开/新建** 组件内进行使用。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **单元格** ：指定填充颜色的目标单元格，可填入单元格地址(如，"A1")或单元格区域（如，"A1：C10"）。此处不可为空，否则运行失败。
- **工作表** ：指定目标单元格所属工作表名称。

### 输出

- **颜色** ：指定填充色(16 进制颜色码)；支持手动输入和从拾色器选择；仅支持字符串变量和字符串

## 使用示例

**前置必要组件**：[打开/新建](../OfficeExcel/OpenExcel.md)

**此流程执行逻辑**：设置指定工作表“Sheet1”中“A1”单元格的背景色为红色。

![配置设置单元格背景色组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/SetCellBackColor2.png)
