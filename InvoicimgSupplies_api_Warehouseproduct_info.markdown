### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=instock_product_info

### **接口说明**
`分页`

### **请求方式**
get

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|ckid       |              |string |仓库id|
|productid  |              |string |产品id|
### **其他参数**
无
### **浏览器查看**
产品基本信息 http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=instock_product_info&productid=135&access_token=e133ac84d35628422ca6c2c408667a&p=1


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|proList    |         | array |基本信息数组 |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|storn|       | array | 仓库详细 |


### **浏览器查看**
产品出入库流水 http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=supplies_stron_outin&productid=132&access_token=b97c4b2f541b4dbf485ead62553844&p=1&ckid=0

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data|       | array | 数组|
|count|       | int| 总条数|






### **浏览器查看**
批次信息 http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=instock_probatchlist_info&productid=135&ckid=1&access_token=e133ac84d35628422ca6c2c408667a


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data|       | array | 入库批次数组 |
|count|       | string | 条数 |



``` javascript
proList: [
{
ckID: "*",
subTypeId: "278",
maxhidden: false,
minhidden: false,
param0: "大",
param1: "10",
num: "60.00",
format: "FG_-D-10_0"
},
{
ckID: "*",
subTypeId: "279",
maxhidden: false,
minhidden: false,
param0: "小",
param1: "10",
num: "76.00",
format: "FG_-X-10_1"
}
],
tableHeader: {
param0: "包装",
param1: "长度"
},
infos: {
ckname: "全部仓库",
productName: "分割"
},
log: [
{
id: "863",
orderid: "1545",
proid: "135",
subid: "279",
num: "1",
adminUid: "1",
c_time: "1458288050",
stornhouseid: "2",
type: "订单入库",
from: "0",
mark: "sf",
default1: "0",
default: "0",
f3f66: "sdsdas",
param0: "小",
param1: "10",
ggNum: 2,
tag: "+",
froms: "订单操作",
price: "23.00",
format: "FG_-X-10_1",
admin: "庆丰包子",
time: "2016-03-18 16:00"
},
``` javascript
{
storn: [
{
id: "1",
storehouse: "武汉仓库(默认仓库)",
default1: "0",
defaultStore: "1",
warehouse: [
{
id: "27",
storehouse: "库位C(默认库位)",
default1: "1",
defaultStore: "1",
product: [
{
param0: "大",
param1: "10",
formatNum: 60,
formaname: "FG_-D-10_0"
},
{
param0: "小",
param1: "10",
formatNum: 73,
formaname: "FG_-X-10_1"
}
]
}
]
},
{
id: "2",
storehouse: "北京仓库",
default1: "0",
defaultStore: "0",
warehouse: null,
product: [
{
param0: "小",
param1: "10",
formatNum: 2,
formaname: "FG_-X-10_1"
}
]
},
{
id: "31",
storehouse: "测试仓库",
default1: "0",
defaultStore: "0",
warehouse: null,
product: [
{
param0: "小",
param1: "10",
formatNum: 1,
formaname: "FG_-X-10_1"
}
]
}
]
}
