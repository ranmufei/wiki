# 报销单详情
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=bxinfo

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=bxinfo&id=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 报销id |

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|pj|array |array|数组|
|yj||int|yj为1时显示yjian这个字段|
|statu||int|statu为1时就有审核框和审核意见|
|data||array|报销票据的数据（为空就没有数据)|
|documentid||string|票据号|
|money ||string|金额|
|fileid||string|图片的路径:”./Uploads/2015/0515/17/5555bad8752ce.png”|
|time  ||string|票据的时间|
|isreceipt| 是/否 |sring|是否为票据|
|documentname|  |string|票据名称|
|cateid|  |string|类别名称|
|projectid|  |string|项目名称|
|docbz|  |string|备注|


### 实例

``` javascript
{
pj: {
yj: null,
statu: 0,
data: [
{
documentsid: "1431594688179669",
money: "1212.00",
fileid: "./Uploads/2015/0514/17/555466c0a4778.png",
cateid: "差旅费",
projectid: "项目3",
time: "2015-05-14 17:11:28",
isreceipt: "是",
documentsname: "阿什顿",
docbz: "无"
}
]
},
bx: {
id: "58",
userid: "庆丰包子",
expenseid: "2015051598564850",
time: "2015-05-15 15:02:19",
estatus: "已报销",
isdelete: "0",
expensename: "十大",
bz: "阿什顿",
yjian: "",
default1: "",
default2: "",
money: 1212
},
history: {
cwu: [
{
amount: "1.00",
inputtime: "2015-05-21 16:30",
userid: "1",
username: "庆丰包子"
},
{
amount: "1.00",
inputtime: "2015-05-21 16:21",
userid: "1",
username: "庆丰包子"
}
],
his: [
{
userid: "庆丰包子",
time: "2015-05-21 16:30:54",
status: "财务已审核"
}
]
}
}