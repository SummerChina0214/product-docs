# 错误捕捉（Try Catch）

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/TryCatch.mp4"></video>

## 概述

针对异常处理，能够捕获流程图或组件中的指定异常类型，并显示错误通知或继续执行。由三部分组成：

- **Try** ：组件执行过程中可能抛出的异常
- **Catches** ：抛出异常时的处理方案
    - **Exception**：捕捉的异常类型，可添加多个
- **Finally** ：在组件结束时执行

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

## 使用示例

**此流程执行逻辑**：通过try容器中点击过list中第一个元素后，当前页面会跳转为其他页面，导致循环点击list的其他元素时失败，为此我们在catch中设置跳转为初始页面，以此来初始化页面从而可正常点击list中其他元素。

![配置错误捕捉组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/tryCatch-4.png)

## 常见问题

1. **Q：如果触发了异常，如何在当前循环再执行一次Try里面的流程？**

    ![trycatch](https://docimages.blob.core.chinacloudapi.cn/images/Activities/trycatch20210825.png)

    **A：** Try里面用重试包一个一次地重试，在抛异常出去之前会重试一次，重试还是失败后才往外抛异常。

    ![示例](https://docimages.blob.core.chinacloudapi.cn/images/Activities/trycatch120210825.png)
