# 高亮

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/Highlight.mp4"></video>

## 概述

将指定元素高亮，可选择颜色和时间。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **颜色** ：指定高亮的颜色
- **高亮时长（毫秒）** ：高亮的时长，1000ms = 1s。

### 目标

- **控件元素** ：接收变量作为目标元素。属性 **控件元素** 和 **选择器** 二者互斥。
- **[选择器](../Appendix/Selector.md?_v=v2020.4)** ：要获取的特定 UI 元素。可通过点击 **指定元素** 自动生成。仅支持字符串变量和字符串
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待，1000ms = 1s。

## 使用示例

**此流程执行结果**：将指定的元素呈黄色高亮 1 秒时长。

![配置高亮组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/highlight1.png)
