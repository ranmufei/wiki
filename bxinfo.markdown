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
|一级pjdata||array|报销票据的数据（为空就没有数据)|
|二级documentid||string|票据号|
|二级money ||string|金额|
|二级fileid||string|图片的路径:”./Uploads/2015/0515/17/5555bad8752ce.png”|
|二级time  ||string|票据的时间|
|二级isreceipt| 是/否 |sring|是否为票据|
|二级cumentname|  |string|票据名称|
|二级cateid|  |string|类别名称|
|二级projectid|  |string|项目名称|
|二级docbz|  |string|备注|
 
|一级bx|array |array|报销详情数组|
|----|----|----|-----|
|二级id||int|报销id|
|二级expenseid||string|报销号|
|二级money||string|金额|
|二级userid||string|申请人|
|二级estatus||string|状态|
|二级time||string|票据的时间|
|二级expensename||string|报销名称|
|二级bz||string|备注|
|二级yjian||string|审核人意见|

|一级history|array |array|记录数组|
|----|----|----|-----|
|二级cwu||array |付款记录数组|
|三级amount|  |string|金额|
|三级inputtime|  |string|时间|
|三级username|  |string|操作人|
|二级his||array|审批记录|
|三级time|  |string|时间|
|三级inputtime|  |string|操作人|
|三级status|  |string|状态|

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