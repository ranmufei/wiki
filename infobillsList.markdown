### **请求方式**
get/post

### **浏览器查看（我的对账单详情列表）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mygysbill&p=1&access_token=

### **浏览器查看（对账单详情列表）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=gysbill&p=1&access_token=

### **公共参数** 
`num`、`p`

### **其他参数**

timestart  筛选的开始时间（我的对账单、对账单）
timeend    筛选的结束时间 （我的对账单、对账单）
userid     筛选的员工 （对账单）


### **返回结果（如下）**



``` javascript
//没有数据 的情况（count: 0  ）
{
data: {
count: 0,
totalPages: 0,
nowPage: 1,
data: ""
},
info: {
count: 0,
num: 0,
money: 0,
pay: 0,
nopay: 0
},
gys_name: "Hahhahahha"
}

//有数据的情况
{
data: {
count: "1",
totalPages: 1,
nowPage: 1,
data: [
{
id: "1448",
uid: "1",
gys_id: "408",
order_num: "XS2016030898975299",    //销售单号
creat_time: "03-08 14:33",           // 创建时间
to_time: " ",
count_price: 33600,          //订单金额
ml_price: "0.00",
ordertype: "2",
from: "14",
mark: "2222",
default6: "0",
is_bigorder: "0",
is_xs: 0,
is_open: 0,
uname: "庆丰包子",          //开单人
gys_name: "Hahhahahha",       //客户
num: "168.00",
type: "销售",   //订单类型
havePay: "0.00",         //已收金额
nopay: 33600          //待收金额
}
]
},
info: {
count: 1,
num: 168,
money: 33600,          //订单应收 
pay: 0,               //已收金额 
nopay: 33600          //待收金额 
},
gys_name: "Hahhahahha"
}