# 报销列表
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=bxlist

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=bxlist&uid=1&status=1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
| status| 是 | 报销单状态id,不传参默认为0，查询的是所有的|


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
expenseid: "2015060856574957",
money: "15.00元",
userid: "庆丰包子",
estatus: "审核中",
time: "2015-06-08 17:42:32",
expensename: "测试",

}]
