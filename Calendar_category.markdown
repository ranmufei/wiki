# 受邀日程列表
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_category

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_category



## 返回结果

返回数据见实例

###实例
``` javascript

[
{
id: "1",//分类id
important: "一般",//优先级
color: "#cfa36d",//背景颜色
textColor: "#ffffff",//文本颜色
uid: "1",//用户id
count: 11//该分类使用总数
},
{
id: "2",
important: "紧急",
color: "#e9be49",
textColor: "#ffffff",
uid: "1",
count: 14
},
{
id: "5",
important: "非常重要",
color: "green",
textColor: "write",
uid: "1",
count: 7
},
{
id: "6",
important: "特别重要",
color: "#feff8f",
textColor: "#f95280",
uid: "1",
count: 3
},
{
id: "7",
important: "不重要",
color: "#000000",
textColor: "#ffffff",
uid: "6",
count: 1
},
{
id: "9",
important: "普普通通",
color: "#eadeae",
textColor: "#9e3d3d",
uid: "6",
count: 4
},
{
id: "14",
important: "百度",
color: "#fbfdfe",
textColor: "#cf1616",
uid: "1",
count: 0
}
]
