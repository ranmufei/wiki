## 配制参数说明
- key  : 应用唯一值,应该和应用文件夹名称保持一致,首字母大写
- name ：应用名称
- type : fun:功能应用(请使用此参数); sys:系统应用(不显示在首页,只作为辅助开发调用); 
- use  ：c:公司应用 u个人应用
- prop : 应用属性(vocational:业务与生产; administration:行政与人力; public:公共与财物; marketing:智能营销; community:社区与分享; supplychain:智能供应链)

- 加密`Addons`及`App`文件夹下文件 (其中 `应用/Common/common.php`、`应用/Conf/config.php` `不可加密`)
- 哪些应用是要单独做升级处理,不能使用到发行版的
- `授权地址` 及 `升级包下载地址`是否已改成网络的
- `mobile 端`测试账号清除 Home/Lib/Action/MobileauthAction.class.php 

