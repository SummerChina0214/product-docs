# 复制/移动文件夹

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/MoveOrCopyFolder.mp4"></video>

## 概述

对目标文件夹进行复制或移动至特定位置。效果实现同系统对文件夹的复制和剪切操作。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **复制/移动** ：下拉框选择对文件夹进行复制或移动操作。选择复制，实现将源文件夹副本复制到目的路径；选择移动，实现将源文件夹在源位置删除，移动放置在目标路径，此时仅存在一个文件夹。两者差别在于源路径是否存留源文件夹
- **目标路径** ：目标文件夹放置的目标位置。若出现文件夹同名，则运行失败。
- **源路径** ：复制或移动的目标文件夹。支持相对和绝对路径。可在组件面板点击弹出对话框，选择目标文件夹；亦支持手动输入路径，若路径不存在，则运行失败。

## 使用示例

**此流程执行逻辑**：D盘的文件夹复制到E盘路径下。

![配置复制/移动文件夹组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/moveFolder-1.png)
