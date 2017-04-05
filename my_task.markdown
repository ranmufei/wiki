# 我的任务列表
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=mytask

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=mytask&uid=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id  |
|str| 否| 搜索工作名字段  |
|workState| 是| 列表分类 默认 1  0 所有 1 待审核 2 已审核  |



## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 工作流的总数|

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|工作id|
|text_id||int|对应的存储工作内容表id|
|description||varchar|工作名称|
|lcid||int|对应的流程id|
|uid||int|用户id|
|workerid ||varchar|工作协同者id|
|cid|  |int|公司id|
|endtime|  |int|结束时间|
|status|  |int|工作进行状态（进行中与结束）|
|time|  |int|工作创建时间|
|field|  |int|工作审核状态|
|cz|--|--|操作（数据库中没有该字段）|