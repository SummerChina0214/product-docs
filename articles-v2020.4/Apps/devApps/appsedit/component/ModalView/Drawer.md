# 抽屉

抽屉是可以弹出和隐藏的一个临时的弹出面板。

## 属性

### 配置

- **标题**：设置该组件的标题内容。
- **关闭抽屉**：点击组件的外侧时是否关闭抽屉。
- **内容设置**：当内容超过窗口高度时的执行操作。
- **抽屉尺寸**：抽屉的宽度。

### 事件

- **触发**：通过单击“**新增事件**”按钮，新增事件及对应的行为操作。

  > **说明：**
  >
  > 一个组件可以定义多个不同事件，一个事件可以包含多个相同或不同的行为，多个行为组成一个动作流并按顺序自上而下依次运行。

## 示例

1. 进入 **应用开发** 的编辑模式。
2. 从左侧组件面板中选择 **模态视图** 下的 **抽屉** 组件，拖拽至画布中。
3. 为该组件设置如下属性。

    - 内容：如，`侧边导航`。

4. 为该组件所在的页面配置触发事件。

    - 事件：选择“页面进入”。
    - 行为：选择“打开抽屉”，并指定已设置的抽屉“Drawer”。

5. 单击 **预览** ，查看应用效果。
