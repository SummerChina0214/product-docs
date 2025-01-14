# 读取行/列数据

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/ReadColumnRowDatable.mp4"></video>

## 概述

读取指定工作表中的某一列或某一行，将读取到的内容保存在数组中并可输出。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **读取行/列** ：指定组件操作为读取行或者为读取列。
- **工作表** ：读取的目标行或列所在的工作表。
- **起始单元格** ：读取行或列时的起始单元格。将从此单元格开始，结合“读取行/列”属性所选择的行或列，来横向或者竖向读取数据。

### 输出

- **数组** ：将读取到的数据存储在此变量。

### 可选项

- **保留格式**：勾选时，将同时读取目标单元格的数据内容和数据格式（例如：货币，日期等），并在作为 "写入单元格" 等写入组件的输入时，同时保持此数据格式；不勾选时，在写入时使用默认 "常规" 数据格式。

## 使用示例

**前置必要组件**：[打开/新建](../OfficeExcel/OpenExcel.md)

**此流程执行逻辑**：在 **打开/新建** 组件中，拖入 **读取行/列数据** 组件，读取 sheet1 工作表中 A1 单元格中的数据，通过 **写入行/列数据** 组件写入至 sheet2 工作表中的 A1 单元格中。

![配置读取行/列数据组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadRowOrColumn2.png)
