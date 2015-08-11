# 个人日程列表
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_data

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_data&status=1&uid=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
|status| 是 |呈现1 . 当月, 2 . 本周 , 3 . 当天的所有日程|

## 返回结果

|list|array | array | 返回数据 数组|
|----|----|----|-----|
如实例

###实例
``` javascript

{
count: "3",
totalPages: 1,
nowPage: 1,
data: [
{
id: "448",
uid: "1",
username: "庆丰包子",
cid: "1",
app: "",
createtime: "1437977916",
startime: "1437977940",
endtime: "1438009680",
type: "1",
important: "2",
title: "请问",
content: "12 12",
tixintime: "10",
status: "1",
ident: ""
},
{
id: "449",
uid: "1",
username: "庆丰包子",
cid: "1",
app: "",
createtime: "1437978011",
startime: "1437978060",
endtime: "1438009740",
type: "1",
important: "5",
title: "测试",
content: "测试",
tixintime: "10",
status: "1",
ident: ""
},
{
id: "451",
uid: "1",
username: "庆丰包子",
cid: "1",
app: "",
createtime: "1437979163",
startime: "1437978360",
endtime: "1438151160",
type: "0",
important: "5",
title: "klbj",
content: "hbbjjjjjjjjjjjj",
tixintime: "10",
status: "0",
ident: ""
}
]
}