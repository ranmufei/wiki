实现上传附件的统一调用接口,虽然使用avalon组件模式，但不涉及扫描。(目前仅实现上传的简单功能)  
### 调用方式  
调用组件的元素目前只是起一个触发调出上传组件域的功能，所以开发者可以自由设计。  
HTML中：`<a href="#" ms-widget="upload">上传文件</a>` ,define依赖define(['upload/upload'])  

| 配制参数 |  类型| 默认值 |  描述  |
| :-- | ----:| :--: |
|[新建销售订单(avalon)](creatSaleOrder)| avalon | 创建销售订单 Avalon 组件 |
|[客户选择(avalon)](selcustom) | avalon | avalon组件选择客户 |
|[选择职员(avalon)](member)   | Avalon | 选择职员 |
|[查询条件构造器(avalon)](fieldsearch)| Avalon | 查询条件构造器 |
|[框架公共数据(avalon)](apppublic)| Avalon | 框架公共数据 |
|[选择发货地址](choiceAddressWidgit)| thinkphp | thinkphp 组件选择发货地址 |
|[汉字转拼音码](fz2py)| js + avalon | thinkphp 汉字转拼音首字母 |
|[商品选择控件](choiceProduct)| thinkphp | thinkphp 组件选择进销存产品 |
|[设置右键](settingmenu)| js | js右键下载 |
|[下载监听](downloadAddevenlist)| js | 软件下载文件保存地址接口 |
|[上传组件](upload)|js|以webuploader为核心的上传组件|
