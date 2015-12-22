# 根据点击某一天获取日程及受邀日程
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=get_calendar_schedule

>  method :get/post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=get_calendar_schedule&uid=1&time=2015-12-15&access_token=
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
| time| 是 | 查询某一天的时间|


## 返回结果

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|日程id|
|title||string|日程标题|
|content|  |string|日程内容|
|uid||int|用户id|
|startime||string|开始时间|
|endtime||string|结束时间|




###实例
``` javascript


{
id: "123",
uid: "1",
createtime: "12-15 16:22",
startime: "12-15 16:22",
endtime: "12-16 00:00",
type: "0",
important: "1",
title: "让人",
content: "仿佛刚刚好好好",
tixintime: "0",
workstatus: "0"
},
