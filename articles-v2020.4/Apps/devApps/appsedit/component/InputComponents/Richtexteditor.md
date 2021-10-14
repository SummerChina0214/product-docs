# 富文本编辑框

富文本编辑框是一种可内嵌于浏览器，所见即所得的文本编辑器。它提供类似于Office Word 的编辑功能，方便那些不太懂html用户使用。

## 属性

### 配置

- **默认值**：显示在富文本编辑框中的内容。
- **边距**：设置边距的展现样式。
- **高**：组件的高度。

### 样式

- **隐藏**：组件显示还是隐藏。
- **禁用**：组件禁用还是启用。
- **样式**：可选择“默认样式”，当调整字体、外观、边距时自动显示为“自定义样式”。
- **文字**：设置组件的字体大小、颜色、样式及格式。
- **外观**：设置组件的外观样式。
- **鼠标手势**：当鼠标悬停于该组件上时，显示的鼠标光标的形状。
  
    鼠标手势选项 | 描述
    ---------|----------
    default | 默认光标（通常是一个箭头）。
    text | 此光标指示文本。
    pointer | 光标呈现为指示链接的指针（一只手）。
    not-allowed | 禁止标记(一个被斜线贯穿的圆圈)光标。用于标示请求的操作不允许被执行。
    help | 此光标指示可用的帮助（通常是一个问号或一个气球）。
    move | 此光标指示某对象可被移动。
    progress | 带有沙漏标记的箭头光标。用于标示一个进程正在后台运行。
    grab | 光标呈现为一只手的形状，表示可以抓取某些东西。
    grabbing | 光标呈现为一只手的形状，表示可以抓取住某些东西。
    e-resize | 此光标指示矩形框的边缘可被向右（东）移动。
    n-resize | 此光标指示矩形框的边缘可被向上（北）移动。
    ne-resize | 此光标指示矩形框的边缘可被向上及向右移动（北/东）。
    nw-resize | 此光标指示矩形框的边缘可被向上及向左移动（北/西）。
    none | 没有为元素呈现光标。

- **透明度**：设置该组件的透明度，值越低越透明。

## 示例

1. 进入 **应用开发** 的编辑模式。
2. 从左侧组件面板中选择 **输入组件** 下的 **富文本编辑框** 组件，拖拽至画布中。
3. 按需为该组件设置属性。
4. 单击 **预览** ，查看应用效果。

    ![富文本编辑框](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/richtexteditor20210930.png)