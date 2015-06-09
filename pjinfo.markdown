# 票据详情
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=pjinfo

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=pjinfo&id=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|id| 是| 票据id |

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|id| |int|票据id|
|documentid||string|票据号|
|money ||string|金额|
|fileid||string|图片的路径:”./Uploads/2015/0515/17/5555bad8752ce.png”|
|userid||int|员工|
|status||int|状态|
|time  ||string|票据的时间|
|isreceipt| 是/否 |sring|是否为票据|
|documentname|  |string|票据名称|
|cateid|  |string|类别名称|
|projectid|  |string|项目名称|
|docbz|  |string|备注|
|docbz|  |string|审核意见|


### 实例

``` javascript
{
id: "1",
documentsid: "1428051226",
money: "50.02",
eid: "8",
fileid: "0",
userid: "庆丰包子",
cateid: "餐费",
projectid: "项目1",
status: "已提交",
time: "2015-04-03 16:53:46",
isreceipt: "是",
isdelete: "0",
documentsname: "出差",
docbz: "无",
audityz: "",
default1: "",
default2: ""
}