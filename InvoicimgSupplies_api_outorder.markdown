### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=get_out_order_list

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=get_out_order_list&access_token=e133ac84d35628422ca6c2c408667a&p=1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|str  |          |string | 检索字段  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data    |         | array |数组 |
|count|         | object | 总数 |

``` javascript
count: "32",
totalPages: 2,
nowPage: 1,
data: [
{
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
username: "庆丰包子",
ordertype: "采购退货订单",
custom: "--",
num: 1,
stroname: "武汉仓库--库位C"
},

### **删除订单**

http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=outorder_del&id=1 access_token=e133ac84d35628422ca6c2c408667a