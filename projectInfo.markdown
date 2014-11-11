# 项目详情

> 该接口返回项目详细 和 动态

## 请求接口 

>  *index.php?app=Home&m=ProjectApi&a=projectInfo*

>  method : get/post

> *测试http://www.apps.com/index.php?app=Home&m=ProjectApi&a=projectInfo&pid=15*
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| p  | 否 |  分页 不填安装默认数   |
|num | 否| 动态 列表显示多少条数据 |




## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 一维数组|
|:----|----|----|-----|
id|900|int|编号id|
|uid|2|int|用户id|
|pro_name|党校开发|string| 项目名称 |
|objective|string|string|项目说明|
|time|2013-01-31|date|创建时间|
|end_time|2013-09-3|date|项目截止时间|
|leader|1|int|负责人id|
|user|array|array| 可见用户数组 结合display字段使用 |
|display|0/1|int|公开/私有|
|status|0/1|int|状态| 进行中/ 结束 |
|isOrder|0|int|如果大于0表示服务型订单号 该订单为服务性订单； 等于0表示普通项目管理|
|:----|----|----|-----|
|nid|900|int|编号id|
|notice|strsssda asd|string| 动态消息 |
|time|2013-2-3|string| 发表时间 |
|name|飞飞|string|发表者姓名|
|pro_id|21|int|项目id|


