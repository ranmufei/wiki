# 报销选人
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=selectaudit

>  method : post

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|p| 是|分页 |



## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 人员的总数（有审核权限）|

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|audit| |int|审核人的id|
|name||string|审核人的名字|




### 实例

``` javascript

{
"data":
[
  {"audit":"1",
   "name":"庆丰包子"
  }
 
],
"count":26
}