# 元素探测器

获取Windows桌面上所有进程的UI树元素信息，在树形节点展开的同时智能根据对应的自动化框架获取下一级的元素信息，并且可以生成对应的选择器，同时支持对选择器的编辑，验证及保存回传操作。 

![img](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/uidetector20201208.png)

## 组成

### 1. 指定元素

点击指定元素按钮并指定某元素后，进程树会自动刷新定位到指定元素的所在层级，同时选择器编辑器更新。
### 2. 验证

点击后可用于验证选择器编辑器内容是否可以定位到某元素。如果验证成功，则会高亮该元素同时按钮显示验证通过；验证失败，则该按钮显示验证失败，查看选择器编辑器，可以通过序号前的符号（对号，叉号）来定位出错层级。

>**说明：**
>
>支持验证多个相同的元素，并提示“找到X个。此时高亮的为第Y个”,且支持上下箭头切换，并自动更新 index 和选中当前高亮的元素。

![验证多个相同元素](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/check20201208.png)

### 3. 进程树

显示桌面进程的UI树元素信息。单击某层可展开查看下级，当某行没有三角符号时表明已没有下级。双击某行可实现刷新选择器编辑器。右键单击弹出菜单，含两项：刷新，生成选择器。
### 4. 选择器编辑器

可用来定位元素。支持双击某项，进入编辑模式，同时更改后的选择器支持保存回传到选择器编辑器。单击某项，可以看到右侧的选择器节点详情。
### 5. 属性

显示进程树某项的属性信息。
### 6. 选择器节点

显示选择器某行节点的属性详情，支持识别用户界面元素所需的所有元素并按已应用和未应用状态进行分类展示。
### 7. 预览窗口

当使用图片识别指定某元素时，此窗口出现并展示图片详情。

## 使用元素探测器获取元素 XPath 信息

如果你希望使用 XPath 的形式对元素进行描述，而非使用默认的节点和属性的方式，你可以勾选“生成 XPath ” 选项，然后使用指定元素按钮，重新指定元素。

![img](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/Tutorial/Selector/%E5%85%83%E7%B4%A0%E6%8E%A2%E6%B5%8B%E5%99%A8XPath.jpg)

指定完成后，你可以获得对应元素的 XPath 表达式。

>**说明：**
>
> XPath 选项只支持 Web 元素。
