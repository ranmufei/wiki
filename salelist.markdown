### **请求接口**
/index.php?app=Invoicimg&m=SaleMobile&a=mysaleList

### **接口说明**
`分页`

### **请求方式**
get/post

### **浏览器查看（我的销售订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mysaleList&status=1&access_token=

### **浏览器查看（我的退货订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mysalethList&status=1&access_token=

### **浏览器查看（销售订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=saleList&status=1&access_token=

### **浏览器查看（退货订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=salethList&status=1&access_token=

### **公共参数** 
`num`、`p`

### **其他参数**
status     默认不传查所有的  销售订单（2为待确认  1为待审核   3为审核中 0为审核通过  6为订单作废中 7为已作废 8为预计回款 9为我协同的订单 10为已生成序列号订单） 

str        搜索单号或者客户
timestart  筛选的开始时间
timeend    筛选的结束时间 
userid     筛选的员工 （销售订单、退货订单有）


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------|--------|--------       |
|statu| |||
|data |array  |array  | order_num: 销售单号; gys_name：客户; creat_time:创建时间;count_price:订单金额; num:数量; stornstatu:（出库状态/入库状态）; paystatu:（收款状态/退款状态）; from:订单来源（只有我的销售订单和销售订单显示） |
|info| '' | |   |

``` javascript
[
{
count: 0      //没有数据 的情况
data: ""
nowPage: 1
totalPages: 0

}
]


//有数据的情况
[
{
count: "11",
totalPages: 1,
nowPage: 1,
data: [
{
count_price: 1692
creat_time: "2016-01-11"
default6: "0"
from: "产品订单"
gys_id: "386"
gys_name: "uuuuu"
id: "793"
intoStoreNum: "0.00"
is_bigorder: "0"
is_open: 0
is_xs: 0
ml_price: "0.00"
num: "4.00"
order_num: "XS2016111113836 (<span style="color:red">待修改</span>)"
orderstatu: "2"
ordertype: "2"
paystatu: 0
stornstatu: 0
to_address: null
uid: "1"
}
.....
]
}
]