# 选择票据的接口
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=userpj

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=userpj&uid=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id |

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|id| |int|票据id|
|documentid||string|票据号|
|money ||string|金额|
|documentname|  |string|票据名称|
|cateid|  |string|类别名称|
|projectid|  |string|项目名称|


### 实例

``` javascript
{
count: "2",
data: [
{
id: "106",
documentsid: "2015060856574957",
money: "15.00",
eid: "0",
fileid: "2026",
userid: "1",
cateid: "水电费",
projectid: "项目2",
status: "1",
time: "1433756552",
isreceipt: "2",
isdelete: "0",
documentsname: "测试",
docbz: "",
audityz: "",
default1: "",
default2: ""
},
{
id: "100",
documentsid: "2015060551501001",
money: "15.30",
eid: "0",
fileid: "2015",
userid: "1",
cateid: "销售费",
projectid: "项目2",
status: "1",
time: "1433472691",
isreceipt: "1",
isdelete: "0",
documentsname: "222",
docbz: "",
audityz: "",
default1: "",
default2: ""
}]