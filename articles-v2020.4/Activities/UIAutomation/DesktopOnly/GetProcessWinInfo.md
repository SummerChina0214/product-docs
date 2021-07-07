# 获取进程窗口信息

获取指定进程下指定的属性。

>**说明：**
>
>如果需要获取以管理员权限启动的进程，那么编辑器中的“项目设置”中需要勾选"以管理员权限执行“选项，否则获取不到该进程。

## 属性

### 基本

- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延迟(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延迟(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件

### 输入

- **进程名**：进程名，可使用元素探测器指定元素后，对应ProcessName属性的值，即为进程名。
- **属性名**：在定位到指定进程的基础上，获取指定的属性。

### 输出

- **属性值**：符合条件的输出值存储在此变量中。

## 操作样例

打开仅网页语言不同的两个网页，使用“获取进程窗口信息”组件，获取其中任一浏览器进程的网页标题`Name`属性，以推断另一网页标题。

>**说明：**
>
> 由于页面多语言且每次打开时语言可能和上次不同，所以用来定位窗口的标题会失效。但是，该浏览器进程下只有两个浏览器窗口同时打开，且其中一个标题固定，故可通过此组件来实现反向推断另一个窗口标题的目的，以此来完成后续的操作。

1. 拖入一个“获取进程窗口信息”组件至流程中。
2. 配置“获取进程窗口信息”组件的属性。

    - 进程名：使用“工具 > 元素探测器”工具进行“指定元素”以指定一个已打开的浏览器，找到ProcessName属性的值，如，`chrome.exe`。

    ![获取进程名](https://docimages.blob.core.chinacloudapi.cn/images/Activities/processname20210622.png)

    - 属性名：下拉选择需要获取的属性名称，如，`Name`。
    - 属性值：创建一个字符串数组类型的变量，如，`S`。

3. 拖入一个“写入日志”组件至“获取进程窗口信息”组件的下方。
4. 配置“写入日志”组件的属性。

    - 日志内容：填写日志内容，如，`"获取进程的Name属性为："+S[0]`。

    ![日志内容](https://docimages.blob.core.chinacloudapi.cn/images/Activities/writelog20210622.png)

5. 保存并运行流程。
6. 在输出窗口中查看流程运行结果。

    ![流程运行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/runresult20210622.png)