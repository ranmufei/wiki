## 订单详细

> 订单详情 

## 请求接口

>  http://www.apps.com/index.php?app=Home&m=InvoicingApi&a=orderInfo&id=33

## 请求参数

|参数|类型|必须|说明|
|:---|---|---|---|
|id|int|是|订单id|

## 返回字段详细

|字段|值|类型|说明|
|:---|----|----|----|
|status|success/error|string|请求返回的状态 成功/失败|
|id|33|int|返回的结果订单id|
|order_id|lssv20213123|string|订单单号|
|charge_name|Jiam|string|负责人|
|custom_name|baiducc|string|客户|
|type|1|int|订单状态 1：周期性订单 。其他值 为一次性订单| 
|zqsj|2014-08-4 12:08|date|周期订单时间；周期订单表示一段时间内有时间限制 本字段表示时间范围内|
|goods_info|array|array|产品详细数组|
|googds_info[][product_name]|圆珠笔|string|发货产品名称信息|
|stateArr||array|订单状态数组|
|time|2013-09-23|date|状态确认时间|
|stateName|已确定|string|确认状态|



### 返回实例

```  javascript
{
status: "success",
info: {
id: "33",
order_id: "lssv2014081831",
goods_info: {
94: {
product_name: "圆珠笔",
formats: {
75: {
product_id: 94,
format_id: 75,
num: 419,
format_name: "蓝色*钢制"
}
}
},
95: {
product_name: "24325325",
formats: {
76: {
product_id: 95,
format_id: 76,
num: 49,
format_name: "45"
}
}
},
97: {
product_name: "23452315",
formats: {
78: {
product_id: 97,
format_id: 78,
num: 889,
format_name: "123523*215"
}
}
}
},
userid: "1",
state: "1",
qg_id: "148",
custom_id: "5",
rec_amount: "3123.35",
hav_amount: "0",
charge: "1",
sure_charge: "0",
type: "0",
circle_time: "0",
circle_times: "0",
inputtime: "1408347649",
first_time: "0",
down_id: "1126",
remark: "我去卡卡西肯",
create: "庆丰包子",
charge_name: "庆丰包子",
stateArr: {
state: 1,
stateName: "已确认",
time: "1408347671"
}
}
}

