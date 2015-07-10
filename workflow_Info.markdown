# 工作详情
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=work_list

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=work_list&uid=1&id=185
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id  |
|id| 是| 工作id  |


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



### 实例

``` javascript
{
shid: "1",
dshid: "庆丰包子",
histroy: null,
info: {
id: "185",
text_id: "186",
description: "1",
lcid: "82",
uid: "6",
workerid: "279,286",
cid: "1",
endtime: "0",
status: "进行中...等待庆丰包子审核!",
time: "07-03 14:18",
field: "0",
userid: "谷歌",
times: "2015-07-03 14:18:00"
},
map: {
0: {
cont: "6",
type: "1",
ziduan: 0
},
1: {
cont: "5",
type: "2",
ziduan: 1
},
2: {
cont: "4",
type: "3",
ziduan: 2
},
3: {
cont: "3",
type: "4",
ziduan: 3
},
4: {
cont: "2",
type: "5",
ziduan: 4
},
5: {
cont: "1",
type: "6",
ziduan: 5
},
6: {
cont: "0",
type: "7",
ziduan: 6
},
id: "136"
},
status: "0",
notice: "0",
stamp: "0",
workername: [
"陈丽鹏",
"clp"
],
field: "0"
}