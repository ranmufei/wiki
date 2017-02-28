# 报销单详情
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=bxinfo

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=bxinfo&id=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 报销id |
|status| 是| 报销单状态|

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
|二级projectid|  |string|来源|
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
|三级def|  |string|意见|
|三级inputtime|  |string|操作人|
|三级status|  |string|状态|

### 实例

``` javascript
{
pj: {
selfbh: 1,//为1就显示删除和撤回
statu: 1,//为1就显示审核框和审核意见
count:1,
data: [
{
cateid: "餐费"
docbz: "伽师瓜"
documentsid: "2015091610053979"
documentsname: "手工"
fileid: "./Uploads/2015/0916/10/55f8d4d85a807.png"
isreceipt: "否"
money: "200.00"
projectid: "项目"
time: "2015-09-16 10:33:01"
}
]
},
bx: {
audit: "342"
audits: "张非"//audits不为空就显示  :等待张非审核
bz: "fsdf"
default2: ""
estatus: "审核中"
expenseid: "2015091752549797"
expensename: "sdfsdf"
id: "3"
isdelete: "0"
submit: 1    //为1显示提交按钮
money: 1111
time: "2015-09-17 10:30:12"
userid: "谷歌"
yjian: "sad"
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
cwucount:22,
hiscount:2,
his: [
{
userid: "庆丰包子",
time: "2015-05-21 16:30:54",
status: "财务已审核"
}
]
}
}



> /index.php?app=Account&m=ExpenseApi&a=delete(post传参 id)


> /index.php?app=Account&m=ExpenseApi&a=recallbx(post传参 id)