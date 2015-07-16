# 工作审核
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=agree_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=agree_work&id=184
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id  |
|id| 是| 工作id  |


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|shid|  | int| 最终审核人的id|
|dshid|  | varchar| 最终审核人的姓名|
|status|  | int|工作运行的状态（进行或结束）|
|notice|  | int|判断数组history是否存在（存在为1不存在为0）|
|field|  | int| 工作的审核状态|


|history|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|id| |int|工作信息回复id|
|wk_id||int|对应的工作id|
|mark||varchar|回复的内容|
|uid||int|回复人的id|
|creat_time||int|创建时间|


|info|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|id| |int|工作id|
|text_id||int|对应的存储工作内容表id|
|description||varchar|工作名称|
|lcid||int|对应的流程id|
|uid||int|工作发起者id|
|workerid ||varchar|工作协同者id|
|cid|  |int|公司id|
|endtime|  |int|结束时间|
|status|  |varchar|工作状态显示|
|times|  |int|工作创建时间|
|field|  |int|工作审核状态|
|userid|  |varchar|工作发起者的姓名|

|map|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|cont| |varchar|文本内容|
|type||int|文本框的类型区分|
|ziduan||varchar|文本框的字段（name）|




### 实例

``` javascript