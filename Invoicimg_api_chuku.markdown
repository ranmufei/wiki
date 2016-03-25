### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_order

### **接口说明**
`分页`

### **请求方式**
post

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type       | 默认值2   |string |出库|
|status  |          |string | 0 未入库 1 已入库 2 全部  |
|str  |          |string | 检索字段  |

### **其他参数**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|is_xs=1       |    | |有子单|
### **浏览器查看**
总单列表  http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order&status=2&type=2&access_token=e133ac84d35628422ca6c2c408667a&p=1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id       |    |总单id |出库|
子单查询  http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_z_order&id=1573&access_token=e133ac84d35628422ca6c2c408667a



### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data    |         | array |数组 |
|count|         | object | 总数 |

``` javascript
count: "261",
totalPages: 11,
nowPage: 1,
data: [
{
id: "1560",
uid: "1",
order_num: "XS2016032256539710",
gys_id: "356",
creat_time: "2016-03-22",
count_price: 240,
num: "4.00",
orderstatu: "0",
ordertype: "2",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "0",
default6: "0",
line_status: "0",
is_bigorder: "1",
ordertypes: "销售订单",
gys_name: null,
adminName: "庆丰包子",
intoStoreNum: "0.00",
stornstatu: 0,
is_open: false
},