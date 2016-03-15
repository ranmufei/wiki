### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_order

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order&status=2&type=1&access_token=e133ac84d35628422ca6c2c408667a&p=1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type       | 默认值1   |string |出库|
|status  |          |string | 0 未入库 1 已入库 2 全部  |
|str  |          |string | 检索字段  |
### **其他参数**
无

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
id: "1488",
uid: "1",
order_num: "XS2016031449519810",
gys_id: "422",
creat_time: "1457926529",
count_price: "48000.00",
num: "160",
orderstatu: "0",
ordertype: "2",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "0",
default6: "0",
line_status: "0",
is_bigorder: "0"
},