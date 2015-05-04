## 新员工快速入门


## 项目开发流程

 1 功能设计 （请用流程画图软件 清晰列出功能 参考图如下）

 2  面相 负责人讲解设计的功能 （面相三个以上负责人做功能讲解）

 3 设计数据表 （对功能设计数据表）

 4 功能开发（以上三步功能审核完成后 才可以进行编码工作）


## 学习资料参考

### 前端知识点

- bootstrap 参考：http://www.bootcss.com/

- 项目前端框架 基于bootstrap 参考 http://www.zui.sexy/docs/start.html#intro
 （从5月1号开始之后的新应用前端不在基于zui.css 如需使用 请基于bootstrap ，各位同学请注意）

- avalonjs（非常重要必须学习） 参考 http://www.cnblogs.com/rubylouvre/p/3181291.html

### php框架

- thinkphp


## 公司项目 云盘技术参考


### 函数参考

| 函数名      |    参数 | 返回值  |  说明 |
| :-------- | --------:| :--: |:-------|
| getIP()  | 否 | string   |  返回用户ip地址  例如 201.23.12.33|
| get_avatar()|$uid|string| 根据用户uid 返回用户会员头像地址|
| friendlyDate()|$sTime|string| 格式化时间 返回友好的时间格式 例如 “三分钟之前”。传统时间 2013-10-23 10:20:21|
| getName()|$uid|string| 根据用户uid 返回用户的姓名 |
| getUserName()|$uid|string|根据用户uid 返回用户的账号 切记这个账号是注册账号和姓名不一样 |
| getName()|$uid|string| 根据用户uid 返回用户的姓名 |
| getUserbm()|$jid|string|根据部门jid  返回用部门名称 |
| getUserzw()|$zid|string|根据职位zid  返回用职位名称 |
| getCompanyName()|$cid|string|根据公司cid  返回公司名称 |
| clearArray()|$arr 数组|arrr|删除数组中空字符 空值  |
| appIcon($key,$size)|$key 应用key ,$size 返回应用图片大小（80/32/16）像素|string|应用图片地址  |
| appLink($key)|$key 应用key|string| 获取应用链接地址 |
|  notify($data,$echo=1)|$data   array 消息内容(title,content,link)  ,  $echo   int   是否直接输出|string| 应用发送通知 |
| combination（$arr）|$arr 格式如 Array ( [0] => Array ( [name] => 颜色 [value] => Array ( [0] => 红 [2] => 蓝 [3] => 黑 ) ) ) |string| 生成数组元素的组合 产品多规格通常用到 |
| yuanliaoClass($id)|$id 原料id|string| 原料分类名称 |
| danwei($id)|$id 单位id|string| 返回单位名称 个，元 |
| access_r($uid,$app,$m,$a)|$uid（用户uid）,$app(应用name),$m(模块名),$a（控制器名）|bool| 基于节点的权限判断   例如 access_r(2,Product,Index,dell)  参考建议用tp常量方式获取 模块 控制名 |
| get_03in_companyinfo($cid,$field ='*')|$cid |string| 根据公司cid 获取公司名称  可以获取其他公司名称 |
| app_relyon($name)|$name 应用名称|string| 判断该应用是否有其他应用依赖关系 |
| bool_app_open($key)|$key 应用名称|bool| 应用开启关闭判断|
| nav_string($array,$split ='#')|$arr|string|  导航组装  二种模式 : 1二维数组,链接信息由其中的数组组成,第一个元素为链接名,第二个元素为链接地址; 2一维数组,链接信息由字符串组成,由分隔符隔开,分隔符默认为#号导航组装 $array 二维数组,元素中第一个参数为导航名,第二个为链接地址,如果元素中没有链接,则a=javascript:|



### 更多功能函数参考

* 公共函数以及公共模型查询  http://192.168.1.240/ranmufei/pubic-model/tree/master



## 组件


详细请 查看 组件分类 



## 产品功能设计参考


![进销存pig](http://192.168.1.240/uploads/ranmufei/apps/1d864819e6/%E8%BF%9B%E9%94%80%E5%AD%98pig.jpg)
![databasesDesgin](http://192.168.1.240/uploads/ranmufei/apps/1071e4f873/databasesDesgin.png)
