>    这是一个文档系统 以后 可以在这里发布接口 和分享一些有用的技术资料，欢迎大家一起更新


# 开发帮助

* [升级包升级常见问题及注意事项](sql_error)

* [内部开发环境帮助说明](devHelp)

* [内部测试环境](serviertest)

* [私有盘系统开发说明](privateDev)

* [操作系统配置](syscorntab)

* [私有盘重置说明](resetPrvate)

* [新人快速入门](newstar)

* [avalon 组件开发模板参考](avalon_widget_create)

* [git 密钥生成参考](http://blog.csdn.net/wfdtxz/article/details/8678982)

* [linksame 文档](linksame_document)

* [rancher 开发相关帮助](rancher-dev)

### [v7.0 已上线的应用](onlineApp)

### [发行及升级](versionorupdate)

### [应用配制](appconfigdesc)

### [应用初始化功能](appinitguopong)

### [云平台PCD通讯设计](pcdtoclouddesign)

### [系统设置的全局数据调用](pcd_system_to_globaldata)

### [无需登录控制器基类](nopowercontrollerbaseAction)

### [写javascript插件的一些基本规则](write_javascript_plugin_rule )

### [移动端文档 ](mobile_document)
### [PCD引用Linksame页面](pcdaddls)

### **[插件开发](plugindev)**
### **[附件地址 ](attach_address)**

# 私有盘硬件文档
 
   - [技嘉主板 centos 系统无法启动处理](centosDoc)
## [招聘技术提问](ask)
## [公共模型](staticmodel)

* [汉字转拼音PHP](fztopy)
* [初始化数据写在配置文件中](Initial_config)
* [云应用授权SDK文档](sdk)
* [富文本编辑器，“复制外部网页资源转换至本地资源”和“A标签打开默认浏览器”](filter_text_input)

## [手机短信/电话接口](yunxin)
## [首页消息接口列表](indexMessageApi)

* [首页消息接口说明](indexMessage)
* [应用消息接口说明](appMessage)

# 与linksame官网通信接口

- SnsApi::cApi('Company/userList',$oauthArr);

>  请求接口 SnsApi::cApi('接口地址','数组参数')

-  [微信会员、商城会员、连锁会员与会员中心数据交互接口](vip)
 

# 接口
## * [元数据接口整理](rootAPI) `新 2016-03-25`
## - [移动端API列表](mobileAPI)
## - [移动端需求列表](mobileDemand)
## - [移动端根据cid获取Linksame移动应用列表](webmobile)

# 辅助开发说明
* [私有盘模板在线查阅](http://192.168.1.241/moban/matrix-admin00/)

* [jquery 弹出层插件在线查询文档] (http://192.168.1.241/moban/artDialog/)

* [思维导图在线使用] (http://192.168.1.241/moban/my-mind-master/)

* [LOMOX软件接口文档](LomoxDoc)

* [实现数据定时刷新](timed_task)

# [数据库设计文档](databaseDoc)

- [数据库设计工具建模](desginDataBase)

# 私有盘控件

* - [部分Avalon组件在线预览 案例](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) 

| 组件名称 |  类型  |  描述  |
| :-- | ----:| :--: |
|[统一导入组建(avalon)](uploadnew) `新`  | Avalon | 导入组件 `2016-11-9`|
|[在线Office组件(avalon)](office) `新`  | Avalon | office文档在线查看操作组件 `2016-10-31`|
|[审核流组件(avalon)](getflow) `新`  | Avalon | 应用关联组件 `2016-10-19`|
|[应用关联组件(avalon)](appLibrary) `新`  | Avalon | 应用关联组件 `2016-10-12`|
|[云采购产品组件(avalon)](choseproduct) `新`  | Avalon | 云采购产品组件 `2016-06-29`|
|[万能表单组件(avalon)](form) `新`  | Avalon | 万能表单组件 `2016-05-31`|
|[二维码组件(avalon)](qrcode) `新`  | Avalon | 二维码组件 `2016-05-27`|
|[选择客户(avalon)](choicecustom) `新`  | Avalon | 选择选择客户插件 |
|[选择表情组件(avalon)](face)   | Avalon | 选择表情组件 |
|[选择员工新组件(avalon)](choiceuser)  `新` | Avalon | 选择员工 |
|[分享到企业微圈组件](copytwitter) `新` | avalon | 该组件提供接口 开发者可以吧 有需要分享到微圈的的信息 发布  `2016-03-1更新 可设置组件提示文字` |
|[downLoad服务组件](downLoad) `新` | avalon | downLoad 组件用来优化当前客户端软件 ‘A’ 标签下载文件事件  `2016-01-30更新` |
|[PushReceive服务组件](PushReceive) `新` | avalon | PushReceive用于连接Push服务器，接收消息 和 PHP端的Push描述. (优化WebSocket API)  `2016-01-20更新` |
|[bootstrap开关(avalon)](bootstrap-switch) `新` | avalon | avalon集成Bootstrap 开关（switch）控件  `2016-01-13更新` |
|[进销存选择供应商(avalon)](avalon_supplier) `新` | avalon | 查看所有供应商，根据分类查看供应商，根据产品查看供应商  `2015-12-30更新` |
|[选择发货地址(avalon)](avalon_address) `新` | avalon | 选择客户之后选择客户对应的发货地址  `2015-12-15更新` |
|[应用权限独立配置组件(avalon)](avalon_author) `新` | avalon | 可独立的管理单个应用的节点权限  `2015-12-9更新` |
|[产品规格批次选择组件(avalon)](choicebatch) `新` | avalon | 选择产品规格批次 Avalon 组件  `2015-12-2更新` |
|[序列号查看选择组件(avalon)](choiceSerial) `新` | avalon | 查看/选择 产品序列号 Avalon 组件  `2015-12-2更新` |
|[批次/序列号管理组件(avalon)](avalon_batch) `新` | avalon | 管理批次/序列号的 Avalon 组件  `2015-11-19更新` |
|[选择产品组件(avalon)](avalonChoiceProduct) `新` | avalon | 选择进销存产品 Avalon 组件  `2015-11-19更新` |
|[产品规格管理(avalon)](avalonFormat) `新` | avalon | 增加规格管理 Avalon 组件  `2015-11-3更新` |
|[增加产品(avalon)](avalonCreateproduct) `新` | avalon | 增加产品 Avalon 组件  `2015-11-2更新` |
|[单位管理(avalon)](avalonUnit) `新` | avalon | 单位管理 Avalon 组件  `2015-10-30更新` |
|[仓库管理(avalon)](avalonWarehouse) `新` | avalon | 仓库管理 Avalon 组件  `2015-10-30更新` |
|[新建进销存分类(avalon)](creatclass) `新` | avalon | 新建分类 Avalon 组件  `2015-10-29更新` |
|[新建销售订单(avalon)](creatSaleOrder)| avalon | 创建销售订单 Avalon 组件  `2015-06-29更新`|
|[客户选择(avalon)](selcustom) | avalon | avalon组件选择客户 |
|[选择职员(avalon)](member)   | Avalon | 选择职员 |
|[物流发货(avalon)](logistics)   | Avalon | 物流发货 |
|[查询条件构造器(avalon)](fieldsearch)| Avalon | 查询条件构造器 |
|[框架公共数据(avalon)](apppublic)| Avalon | 框架公共数据 |
|[选择发货地址](choiceAddressWidgit)| thinkphp | thinkphp 组件选择发货地址 |
|[汉字转拼音码](fz2py)| js + avalon | thinkphp 汉字转拼音首字母 |
|[商品选择控件](choiceProduct)| thinkphp | thinkphp 组件选择进销存产品 |
|[设置右键](settingmenu)| js | js右键下载 |
|[下载监听](downloadAddevenlist)| js | 软件下载文件保存地址接口 |
|[上传组件](upload)|js|以webuploader为核心的上传组件|
|[商品添加保修期(avalon)](maintenance)   | Avalon | 商品添加保修期|
|[选择地区](chicecity_widget)|Avalon|选择地址组件,可以配合地区ID在公共模型查地区坐标|







# 应用接口
- [现金流](app-cws)
- [连锁管理](sygl)
- [应用发消息接口](sentmassage)
- [Ims网盘接口](Ims-wangpan)

# 应用开发文档

-[进销存](app_jixniao)

- [应用配置说明](appinforead) `20150828`
- [商品属性和订单属性](property) `20161014`

# 公共函数帮助查询

# [常见问题汇总](questionCollect) 

# 帮助 

 * [markdown 语法](markdownWiki)

 * [wiki语法的使用](wikihelp)
#
