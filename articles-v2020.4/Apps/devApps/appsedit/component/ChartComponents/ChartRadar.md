# 雷达图

雷达图又称蜘蛛网图，是以在同一点开始的轴上显示的三个或更多个变量的二维图表的形式来显示多元数据的方法，它将多个维度的数据量映射到坐标轴上，这些坐标轴起始于同一个圆心点，通常结束于圆周边缘，将同一组的点使用线连接起来就称为了雷达图。 适用于展示三个或更多的维度的变量。

雷达图是专门用来进行多指标体系比较分析的图表，一般用于成绩展示、效果对比量化、多维数据对比等，很多企业使用雷达图来展示企业的经营状况，其展示效果非常直观、清晰、明了。

## 属性

## 配置

- **图表名称**：自定义图表的名称。
- **数据源**：通过编写表达式，设置雷达图中数据的来源。
- **统计字段**：选择数据源中某一字段作为统计数值用。
- **聚合方式**：下拉选择对统计字段的操作，支持累加、计数、平均数、最小值、最大值。
- **维度配置**：配置雷达图的维度，即，该图由几条边组成。
- **颜色**：每一个区域的线条颜色。
- **最大值**：由中心点向外的外圉显示数字的最大值。若此项不填写，则外圈显示数字的最大值为统计数据的最大值（取整）。
- **描述**：对自定义的图表的说明。
- **边距**：勾选“外边距”后，可调整该组件距离上下左右外边框的距离。
- **高**：设置组件的高度。

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
2. 从左侧组件面板中选择 **图表组件** 下的 **雷达图** 组件，拖拽至画布中。
3. 选中该组件，在右侧属性栏为该组件配置如下属性。

    - 图表名称：自定义图表的名称，如，“雷达图”。
    - 数据源：编写一段数据源的数据，如，
  `[{"a":288,"b":190,"c":277,"d":345,"e":290,"f":264,"name":"area1"},{"a":255,"b":188,"c":200,"d":377,"e":300,"f":264,"name":"area1"},{"a":230,"b":200,"c":300,"d":330,"e":254,"f":254,"name":"area2"},{"a":222,"b":132,"c":330,"d":270,"e":266,"f":200,"name":"area2"},{"a":300,"b":277,"c":290,"d":242,"e":300,"f":266,"name":"area3"},{"a":243,"b":234,"c":289,"d":300,"e":278,"f":234,"name":"area3"},{"a":265,"b":398,"c":300,"d":356,"e":245,"f":300,"name":"area4"}]`
     - 统计数据：从数据源中选择可以作为统计的字段，如，`name`。
     - 累加方式：选择为统计字段进行的聚合方式，如，`累加（sum）`。
     - 维护配置：新增雷达图的维护，新增6个变量，如，`dimension-a`、`dimension-b`、`dimension-c`、`dimension-d`、`dimension-e`、`dimension-f`。

4. 单击 **预览** ，查看应用效果。

    ![应用效果](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/chartradar20210604.png)
