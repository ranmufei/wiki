### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_order

### **接口说明**
`分页`

### **请求方式**
post

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type       | 默认值1   |string |出库|
|status  |          |string | 0 未入库 1 已入库 2 全部  |
|str  |          |string | 检索字段  |

### **其他参数**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|is_xs=1  |          |string | 有子单  |



### **浏览器查看**

总单列表 http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order&status=2&type=1&access_token=e133ac84d35628422ca6c2c408667a&p=1


### **浏览器查看**

|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id  |          |string | 总单id|
|type  |          |默认1 | 入库判断|
子单列表 http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_z_order&id=1633&type=1&access_token=e133ac84d35628422ca6c2c408667a&p=1
### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data    |         | array |数组 |
|count|         | object | 总数 |


### **ordertype!=6 && ordertype!=27 && ordertype!=28 && default6==0 显示付款状态**


``` javascript
count: "261",
totalPages: 11,
nowPage: 1,
data: [
{
id: "1553",
uid: "1",
order_num: "CG20163229022",
gys_id: "",
creat_time: "2016-03-22",
count_price: 55180.4,
num: "11.00",
orderstatu: "0",
ordertype: "0",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "0",
default6: "0",
line_status: "0",
is_bigorder: "0",
ordertypes: "采购订单",
gys_name: null,
adminName: "庆丰包子",
intoStoreNum: "0.00",
stornstatu: 0,
is_open: false
},