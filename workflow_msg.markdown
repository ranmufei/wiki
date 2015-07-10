# 发送催促
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=sentmsg

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=sentmsg&id=184
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 工作id  |


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 操作记录的总条数|



|history|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|id| |int|操作记录的id|
|wk_id||varchar|对应的工作的项目名称|
|uid||int|操作记录人的id|
|creat_time||int|操作时间|
|ch||varchar|操作记录人：操作记录内容|





