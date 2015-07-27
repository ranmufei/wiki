# 添加日程
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_add

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_add
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
|status| 是 |呈现当月（本周，当天）的所有日程|

## 返回结果

|list|array | array | 返回数据 数组|
|----|----|----|-----|
如实例

###实例
``` javascript

{
count: "1",
totalPages: 1,
nowPage: 1,
data: [
{
id: "450",
uid: "6",
username: "谷歌",
cid: "1",
app: "",
createtime: "1437978125",
startime: "1437978180",
endtime: "1438009860",
type: "1",
important: "5",
title: "ceshi",
content: "ceshi",
tixintime: "10",
status: "1",
ident: ""
}
]
}