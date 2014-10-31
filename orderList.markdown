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
|state|1/3/ 其他数 |int|状态值 : 待生产出库单/ 已生成出货单 / 出货完成 |


## 案例