# 连接器映射关系管理

连接器映射关系管理用于配置测试连接器与生产连接器的映射关系，当应用上架时，系统会根据当前版本的应用所配置的映射关系，将数据源中的测试连接器自动映射为生产连接器。当该版本应用下架时，则将数据源中的生产连接器自动映射为测试连接器。

在“应用开发”的编辑页面中，单击“连接器”图标，即可进入连接器映射关系管理页面，如下图所示。

![连接器入口](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/connectorpath20210412.png)

## 示例

1. 单击页面中的“编辑”按钮后，可编辑页面信息。
2. 单击页面中的“添加”按钮，选择开发环境的测试连接器与生产环境的生产连接器进行匹配。

   >**说明：**
   >
   >下拉选择框中的连接器，是事先在“云扩RPA控制台 > 数据中心 > 连接管理”中创建且在“应用开发 > 数据”中创建对应的数据源。

   ![连接器匹配](https://docimages.blob.core.chinacloudapi.cn/images/Kris/Apps/connectormatch20210412.png)

3. 单击“保存”按钮，即可保存已配置的连接器映射关系。