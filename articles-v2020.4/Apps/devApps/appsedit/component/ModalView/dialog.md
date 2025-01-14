# 对话框

弹出一个有标题的内容框。

## 属性

### 配置

- **标题**：定义弹出框标题。
- **点击外侧时关闭**：当点击对话框外侧时，是否关闭对话框。
- **对话框尺寸**：自定义对话框的宽度和高度。
- **当内容超过窗口高度时**：当对话框内容超过窗口高度时的响应模式，支持选择“滚动显示内容”和“截断显示内容”。

### 事件

- **触发**：通过单击“**新增事件**”按钮，新增事件及对应的行为操作。

  > **说明：**
  >
  > 一个组件可以定义多个不同事件，一个事件可以包含多个相同或不同的行为，多个行为组成一个动作流并按顺序自上而下依次运行。

## 示例

1. 进入 **应用开发** 的编辑模式。
2. 从左侧组件面板中选择 **模态视图** 下的 **对话框** 组件，拖拽至画布中。
3. 为该组件设置如下属性。

    - 标题：如，`对话框`。

4. 为该组件所在的页面配置触发事件。

    - 事件：选择“页面进入”。
    - 行为：选择“打开弹窗”，并指定已设置的弹窗“dialog”。

5. 单击 **预览** ，查看应用效果。
