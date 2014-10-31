##订单列表

> 客户下的订单发货列表

## 请求接口

> http://www.apps.com/index.php?app=Home&m=InvoicingApi&a=productOrder


## 请求参数


|参数名| 必填| 说明|
|:---|----|----|
|无 | 否| 无 |





## 返回参数


|字段|值|类型|说明|
|:----|----|----|----|
|status|success/error| string | 状态值 |
|info|array|array|返回值|
|id|22|int|订单默认自增id|
|order_id|lssv20140901|string|订单号|
|rec_amount|900.00|float|应收金额|
|state|1/3/ 其他数 |int|状态值 : 待生产出库单/ 已生成出货单 / 出货完成 【切记：状态值的三种状态自行判断】|
|time|2013-09-32 09:12| date | 时间|


## 案例


```  javascript

{
status: "success",
info: [
{
id: "33",
order_id: "lssv2014081831",
rec_amount: "3123.35",
state: "1",
time: "2014-08-18 15:41"
},
{
id: "30",
order_id: "lssv2014081130",
rec_amount: "23123.00",
state: "3",
time: "2014-08-11 18:18"
},
]
}