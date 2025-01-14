# 打开浏览器

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/OpenBrowser.mp4"></video>

## 概述

该组件用于使用浏览器打开指定的 URL。

>**说明**：
>
>该组件也常作为容器。其他的一些网页操作组件，也常放置在该组件中完成。

## 浏览器版本要求

参见 [浏览器版本要求](../Browser/browser-version.md)。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输出

- **浏览器** ：将打开的浏览器类型对象存储到此变量，可作为下一浏览器组件的输入。

### 目标

- **浏览器类型** ：打开的目标浏览器类型。如，Chrome，IE。
- **网址** ：将打开此网址。

### 可选项

- **打开方式**：当浏览器类型为 Chrome、Firefox、Edge 时，可选择打开方式为 Native 和 Selenium（WEB 自动化工具）。
- **等待加载完成** ：勾选时，执行操作之前，等待目标用户界面元素加载完成之后才执行下一个组件操作。
- **结束后关闭** ：勾选时，将在此组件结束后自动关闭浏览器。
  
  > **注意：**
  >
  >若使用静默运行方式，请根据情况，判断是否勾选此选项，否则无法绑定浏览器。

- **静默运行**：当打开方式勾选“Selenium”，同时勾选“静默运行”选项时，可实现流程运行时打开独立浏览器且不可视，即使用户手动操作浏览器也互不干扰。
- **最大化** ：勾选时，可以自动将你指定的浏览器最大化。

## 使用示例

**此流程执行逻辑**：打开指定类型浏览器的指定网址。

![配置打开浏览器组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenBrowser20201221-02.png)

## 常见问题

1. **Q：编辑器如何设置等待页面加载完毕后再进行下一步操作？**

    **A：** “打开浏览器”组件默认勾选“等待加载完成”，可设置等待需要操作的元素出现后再操作。

2. **Q：如果我的操作都是浏览器界面，是否都是双击“打开浏览器”组件，在里面界面添加组件？**

    **A：** 不是，如果打开浏览器不关闭，在外部界面也可以用组件操作浏览器里面的元素。

3. **Q：执行打开浏览器组件之后卡住无法向下执行？**

    ![打开浏览器异常](https://docimages.blob.core.chinacloudapi.cn/images/Activities/openbrowser20210827.png)

    **A：** 打开浏览器中的“结束后关闭”属性取消勾选，然后使用“点击”组件关闭浏览器。

    ![解决方法 ](https://docimages.blob.core.chinacloudapi.cn/images/Activities/endtoclose20210827.png)
