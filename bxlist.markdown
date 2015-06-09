# 报销列表
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=pjlist

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=pjlist&uid=1&status=0
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
| status| 是 | 当前的票据状态id,不传参默认为0，查询的是所有的|


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 票据的总数|

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id|      |int|票据id|
|documentid| |string|票据号|
|money |  |string|金额|
|userid|  |int|员工|
|status|  |int|状态|
|time  |    |string|票据的时间|
|isreceipt| 是/否 |sring|是否为票据|
|documentname|  |string|票据名称|
|pc|  |string|类别+票据|

### 实例

``` javascript
{
count: "1",
data: [
{
id: "106",
documentsid: "2015060856574957",
money: "15.00元",
eid: "0",
fileid: "2026",
userid: "庆丰包子",
cateid: "4",
projectid: "2",
status: "已录入",
time: "2015-06-08 17:42:32",
isreceipt: "否",
isdelete: "0",
documentsname: "测试",
docbz: "",
audityz: "",
default1: "",
default2: "",
pc: "水电费+项目2"
}]
