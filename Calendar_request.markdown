# 受邀日程列表
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_request

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_request&uid=1&start=1435507200&end=1438272000
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |


## 返回结果

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|日程id|
|title||string|日程标题|
|uid||int|用户id|
|start||string|开始时间|
|end||string|结束时间|
|type  ||int|日程类型|
|tixintime|  |int|提前通知时间|
|important|  |int|日程的优先级别（对应日程分类表id）|
|content|  |string|日程内容|
|color|  |string|日程事件显示的背景颜色|
|textColor|  |string|日程事件显示的文本颜色|
###实例
``` javascript

[
{
id: "134",
title: "456456",
uid: "1",
start: "2015-06-29 17:48:00",
type: "0",
tixintime: "5",
important: "1",
end: "2015-06-29 17:58:00",
content: "qweqweqweqwe",
color: "#c85058",
textColor: "#ffffff"
}
]
