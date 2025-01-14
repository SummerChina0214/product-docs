# 读取 CSV 文件

## 视频示例

## 概述

将一个 CSV 文件读取，存储到数据表变量。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 输入

- **文件路径** ：要读取的 CSV 文件路径。支持相对和绝对路径。可在组件面板点击弹出对话框，选择目标文件；亦支持手动输入路径，若路径不存在，则运行失败会报错。

### 输出

- **数据表** ：将输入的 CSV 文件存储到此变量，并可取此变量进行数据表相关组件进行操作。

### 可选项

- **编码方式** ：文件的编码方式。可以在 [此处](../Appendix/Encoding.md) 找到每个字符编码的完整代码列表。要指定要使用的编码类型，请使用&quot; 名称&quot; 字段中的值。如果未指定编码类型，则活动将搜索文件的字节顺序标记以检测编码。如果未检测到字节顺序标记，则默认选择 UTF-8。
- **分隔符** ：指定 CSV 文件的分隔符。此属性可不填写，默认使用逗号。
- **列名重复加一**：勾选后，若出现重复列名则在原列名后加下划线和数字（默认是 1，如果依然重复则+2，依次类推），如：原列名_N。

## 使用示例

**此流程执行逻辑**：读取指定的 CSV 文件内容 "C:\云扩科技\savetable.csv"，输出至 `table` 变量中。

![配置读取 CSV 文件组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadCSV20201229.png)
