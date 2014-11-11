# 项目列表

> 该接口返回全公司项目

## 请求接口 

>  *index.php?app=Home&m=ProjectApi&a=projectList*

>  method : get/post

> **测试 http://www.apps.com/index.php?app=Home&m=ProjectApi&a=projectList&num=4&p=2 **
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| p  | 否 |  分页 不填安装默认数   |
|num | 否| 列表显示多少条数据 |



## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|list|array | array | 返回数据 数组|
|:----|----|----|-----|
|id|900|int|编号id|
|uid|2|int|用户id|
|pro_name|党校开发|string| 项目名称 |
|objective|string|string|项目说明|
|time|2013-01-31|date|创建时间|
|end_time|2013-09-3|date|项目截止时间|
|leader|1|int|负责人id|
|user|2,32|string|邀请通知的同事id|
|display|0/1|int|显示/隐藏|
|status|0/1|int|状态| 进行中/ 结束 |
|isOrder|0|int|如果大于0表示服务型订单号 该订单为服务性订单； 等于0表示普通项目管理|
|nd|int|12|需求帖子数|
|tsk|int|23|任务条数|
|tst|int|23|测试调试|
|svr|int|23|服务支持条数|
|dt|int|233|当前项目消息动态回复数|
|:----|----|----|-----|
|count|int|23|列表项目总数 计算分页是 可能会用到|



