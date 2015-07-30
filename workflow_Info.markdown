# 工作详情
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=work_list

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=work_list&uid=1&id=184
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

# 结束工作
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=end_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=end_work
| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id  |
|id| 是| 工作id  |
### 实例

``` javascript
{
shid: "6",
dshid: "谷歌",
histroy: [
{
id: "382",
wk_id: "184",
bz_id: "0",
mark: "ok",
uid: "陈丽鹏",
creat_time: "2015-07-02 15:24:13"
},
{
id: "383",
wk_id: "184",
bz_id: "0",
mark: "ok",
uid: "clp",
creat_time: "2015-07-02 15:24:52"
}
],
info: {
id: "184",
text_id: "185",
description: "采购",
lcid: "82",
uid: "1",
workerid: "279,286",
cid: "1",
endtime: "0",
status: "进行中...等待谷歌审核!",
time: "07-02 15:23",
field: "1",
userid: "庆丰包子",
times: "2015-07-02 15:23:04"
},
map: {
0: {
cont: "2",
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
notice: "1",
stamp: null,
workername: [
"陈丽鹏",
"clp"
],
field: "1"
}