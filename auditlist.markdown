### **请求接口**
/index.php?app=Invoicimg&m=SaleMobile&a=auditlist

### **接口说明**
`分页`

### **请求方式**
get/post

### **浏览器查看（我的对账单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=auditlist&p=1&status=1&access_token=


### **公共参数** 
`num`、`p`

### **其他参数**
status     状态（未审核1，已审核2）
str        搜索单号或者客户
timestart  筛选的开始时间
timeend    筛选的结束时间 
userid     筛选的员工 


### **返回结果**

``` javascript
//没有数据 的情况（info: "error"、statu: 0   ）
[
{    
statu: 0,
info: "error",
data: null
}
]

//有数据的情况
{
statu: 1,
info: "ok",
data: {
count: 2,
data: [
{
id: "1475",
order_num: "DG201603111939284091 (<span style="color:gray">待审核</span>)",   //销售单号
shenh_uid: "1",
gys_id: "420",
creat_time: "2016-03-11",  //创建时间
uid: "1",
ordertype: "2",
orderstatu: "1",
from: "网络销售订单",
count_price: 122100,     //订单金额
default6: "0",
is_bigorder: "0",
is_xs: 0,
is_open: 0,
gys_name: "武汉邻商在线(线上客户)",    //客户
num: "100.00",
intoStoreNum: "0.00",
stornstatu: 0,
paystatu: 0
}
]
}
}