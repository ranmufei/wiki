# 我的工作流列表
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=work_index

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=work_index&uid=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id  |
| status| 否 | 工作状态,不传参默认为2，查询的是所有的|


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 报销的总数|

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|报销id|
|expenseid||string|报销号|
|money ||string|金额|
|userid||string|员工|
|estatus||string|状态|
|time  ||string|报销的时间|
|expensename|  |string|报销名称|


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
