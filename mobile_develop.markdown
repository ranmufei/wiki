## 移动端开发者(android 或 IOS)

* 身份验证 必须带上 登录时 服务器返回的 验证码，服务器会根据验证码判断出用户身份,所以传不传 用户uid则无关要紧了。不过考虑到对以前 接口的兼容性，是否传uid 请移动端开发者 判断
* 服务器框架对 请求参数 做了兼容性处理,所以一个接口中,参数可以完全POST或GET,程序员不再需要根据 参数 的特性，自己来区分。
*

|  |  类型  |  描述  |
| :-- | ----:| :--: |
|[新建销售订单(avalon)](creatSaleOrder)| avalon | 创建销售订单 Avalon 组件  `2015-06-29更新`|
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