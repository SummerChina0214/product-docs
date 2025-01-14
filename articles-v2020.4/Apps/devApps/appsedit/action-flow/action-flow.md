# 动作流

## 概述

**动作流** 用于自定义应用业务逻辑，帮助完成复杂交互。在动作流内，你可以进行执行流程部署、打开新页面或消息通知等操作。

动作流分为可视化动作流和 JS 代码两种呈现形式，可视化动作流则是 JS 代码的可视化表现方式，用户能够通过拖拉拽组件的方式，对一系列动作进行编排，简单快速搭建业务流程。

## 创建可视化动作流

1. 单击“动作流面板”右上角的“+”，选择“可视化动作流”，填写创建的动作流名称。

    ![创建可视化动作流](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/createvisiualflow20220105.png)

2. 拖入左侧“动作流组件”面板中的组件至页面右侧编辑区。

    ![拖入动作流组件](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/actionflow20220105.png)

3. 创建完成的动作流，单击页面上方的“执行”图标，查看运行结果。

## 创建 JS 代码

1. 单击“动作流面板”右上角的“+”，选择“JS 代码”，填写创建的 JS 代码名称。

    ![创建 JS 代码](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/createactionflow20220105.png)

2. 在页面右侧弹框中输入需要执行的 JavaScript 代码。

    > **说明：**
    >
    > 在输入 JavaScript 代码时，会自动提示并高亮代码。

    ![输入 js](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/javascriptcode20210325.png)

3. 编写完成的代码，单击“运行”按钮，可测试查看运行结果。

    ![执行结果](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/javascriptcoderesult20210325.png)

4. 单击“保存”按钮。

## 调用动作流

1. 在 ViCode 的大纲页面，拖入页面组件至编辑区。
2. 选择需要触发动作流事件的组件，在“事件”属性中，关联已创建完成的可视化动作流或 JS 代码。

    ![调用动作流](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/invokeactionflow20220105.png)
