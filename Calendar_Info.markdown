# 日程详情
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_list

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_list&uid=1&id=198
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
| start| 是 | 查询日程的起始时间|
| end| 是 | 查询日程的结束时间|

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
|important_name|  |string|日程的优先级别（对应日程分类名称）|
|content|  |string|日程内容|
|color|  |string|日程事件显示的背景颜色|
|textColor|  |string|日程事件显示的文本颜色|


|list|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|回复内容id|
|r_id| |int|对应的日程id|
|uid||int|用户id|
|u_name||string|用户名称|
|comment||string|回复内容|
|time||string|回复时间|
|src||string|用户头像对应的地址|




###实例
``` javascript


{
array: {
id: "198",
title: "打卡",
start: "2015-07-10 18:38:00",
type: "工作日程",
tixintime: "10",
important: "9",
important_name: "普普通通",
uid: "1",
end: "2015-07-10 21:38:00",
content: "打卡"
},
list: [
{
id: "302",
r_id: "198",
uid: "6",
u_name: "谷歌",
comment: "打卡没有啊？？",
time: "07-11 11:22:29",
src: "./Uploads/avatar/0/6.jpg"
}
]
}
