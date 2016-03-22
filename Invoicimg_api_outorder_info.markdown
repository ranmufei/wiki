### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=get_outorder_info

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_outorder_info&access_token=e133ac84d35628422ca6c2c408667a

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id|              |string | 出库订单id  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|orderinfo|         | object|订单基本信息 |
|list|         | array| 产品信息|
|wuliudetail|         | array | 物流订单信息 |
|wuliudetail[0][wl_dynamic]|         | array | 物流动态|
|piciInfo|         | array | 批次记录 |
|xulieInfo|       | array | 序列号记录 |

``` javascript
{
orderinfo: {
id: "32",
number: "CK201603222810",
order_id: "1551",
sort: "0",
time: "2016-03-22 10:13",
stron_id: "27",
uid: "1",
default: "1",
isDelete: "0",
default2: null,
default3: null,
stroname: "武汉仓库--库位C",
username: "庆丰包子",
custom: null,
ordertype: "1",
to_time: "2016-03-22",
address: "辽宁省/丹东市/元宝区/阿斯顿",
receiver: "阿斯顿",
phone: "13545698745",
mobile: "13545698745",
num: 1
},
list: [
{
id: "37",
o_id: "32",
pro_id: "157",
formatid: "390",
num: "1",
product: "萨达萨达啊",
format: "SDSDA",
chukumoney: "45.00"
}
],
wuliudetail: [
{
id: "40",
express_number: "375191712435",
uid: "1",
d_address: "武汉",
delivery_time: "1458613105",
delivery_img: null,
company_id: "33",
addressee_name: "阿斯顿",
s_uid: null,
addressee_phone: "13545698745",
address: "辽宁省/丹东市/元宝区/阿斯顿",
addressee_company: "柯斯达",
log_money: "13",
expected_time: "1459353600",
actual_time: null,
status: "1",
logistics_id: "0",
stamp: "0",
delete: "0",
is_delete: "0",
default2: "阿斯顿啊",
company: "中通快递",
product_data: [
{
id: "51",
num: "1",
product: "萨达萨达啊",
order_id: "38",
orderid: "32",
product_id: "37",
status: "1",
statu: "1",
e_id: "0"
}
],
wl_dynamic: [
{
time: "2016-01-23 17:52:07",
location: "",
context: "[汉阳] 派件已 签收 ,签收人是拍照签收签收网点是汉阳",
ftime: "2016-01-23 17:52:07"
},
{
time: "2016-01-23 09:06:15",
location: "",
context: "[汉阳] 汉阳的汤润刚正在派件",
ftime: "2016-01-23 09:06:15"
},
{
time: "2016-01-23 02:51:39",
location: "",
context: "[汉阳] 快件到达汉阳,上一站是武汉中转部 目的地是",
ftime: "2016-01-23 02:51:39"
},
{
time: "2016-01-22 23:27:39",
location: "",
context: "[武汉中转部] 快件在武汉中转部装车,正发往汉阳",
ftime: "2016-01-22 23:27:39"
},
{
time: "2016-01-22 22:54:35",
location: "",
context: "[武汉中转部] 浙A6M027已经到达武汉中转部",
ftime: "2016-01-22 22:54:35"
},
{
time: "2016-01-21 23:02:41",
location: "",
context: "[金华中转部] 浙A6M027在金华中转部已发车，下一站武汉中转部，",
ftime: "2016-01-21 23:02:41"
},
{
time: "2016-01-21 22:17:30",
location: "",
context: "[金华中转部] 快件在金华中转部装车,正发往武汉中转部",
ftime: "2016-01-21 22:17:30"
},
{
time: "2016-01-21 22:13:35",
location: "",
context: "[金华中转部] 快件到达金华中转部,上一站是浦江黄宅目的地是武汉",
ftime: "2016-01-21 22:13:35"
},
{
time: "2016-01-21 19:13:31",
location: "",
context: "[浦江黄宅] 快件在浦江黄宅,正发往金华中转部",
ftime: "2016-01-21 19:13:31"
},
{
time: "2016-01-21 19:12:45",
location: "",
context: "[浦江黄宅] 快件在浦江黄宅装车,正发往金华中转部",
ftime: "2016-01-21 19:12:45"
},
{
time: "2016-01-21 19:09:22",
location: "",
context: "[浦江黄宅] 浦江黄宅 的 朱一军 已收件 ",
ftime: "2016-01-21 19:09:22"
}
]
}
],
piciInfo: [ ],
xulieInfo: [ ]
}