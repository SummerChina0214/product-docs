# 发送邮件(SMTP)

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/SendSMTPMail.mp4"></video>

## 概述

使用 SMTP 服务自动检测加密方法发送邮件，同时可使用代理。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 发件人

- **密码** ：发件人邮箱的密码。
- **邮箱地址** ：使用此邮箱地址作为发件人，执行发送邮件操作。

### 服务器

- **代理** ：发送邮件时若要使用代理，则填充此属性；格式为【服务器：端口号】。
- **端口号** ：发送邮件时所经端口号。如，587。
- **服务器** ：发件人邮箱所属服务器地址。如，“smtp.×××.outlook.cn”。

### 邮件

- **HTML 格式** ：说明邮件内容是否时 HTML 格式，若勾选后，则按照 HTML 格式处理邮件内容。
- **抄送人** ：发送邮件时的抄送人邮箱地址。可写多个收件人，用分号分割即可；例如：`user1@encootech.com; user2@encootech.com`。
- **附件** ：发送邮件的附件。支持相对和绝对路径。可写多个附件地址，具体写法参考：new List <string>(){"文件 1 路径", "文件 2 路径"}，也可以点击 "..." 在弹窗中选择文件后自动生成。
- **密件抄送** ：发送邮件时的密件抄送人邮箱地址。可写多个收件人，用分号分割即可；例如：`user1@encootech.com; user2@encootech.com`。
- **收件人** ：邮件接收人邮箱地址。可写多个收件人，用分号分割即可；例如：`user1@encootech.com; user2@encootech.com`。
- **邮件内容** ：发送邮件的正文内容。如，“云扩科技：发送邮件（SMTP）”。
- **邮件主题** ：发送邮件的主题。如，"发送邮件（SMTP）"。
- **重要性**：选择邮件的重要等级，包括正常、高、低。

### 可选项

- **安全连接** ：指定检测加密方法，默认为自动。
- **超时**：指定此组件的执行时间。若超出此时间，组件还未执行，会抛出错误。

## 使用示例

**此流程执行逻辑**：使用 SMTP 服务，将邮件内容发送给指定的收件人。

 ![配置发送邮件(SMTP)组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/SendMailSMTP2020122202.png)
