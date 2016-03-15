### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_product_list

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
/http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_product_list&access_token=

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|ckid       |              |string |根据仓库查询仓库产品库存|
|str        |              |string | 检索字段  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript
{
id: "157",
uid: "1",
cid: "1",
cate_id: "83",
name: "萨达萨达啊",//产品名
code: "SDSDA",
formatType: "1",
brand: "456",
SupplierId: "2",
unitInfo: "0",
shelfLife: "0",
isDelete: "0",
b_no: null,
xinhao: null,
h_id: null,
unit: "",
price: "0.00",
count_price: "0.00",
time: "1457942089",
num: "100.00",//库存数量
max_limit: "0",
min_limit: "0",
mark: "456",
status: "0",
sns_id: null,
default2: "0",
default1: "0",
form: "0",
productName: "萨达萨达啊",
produckID: "157",
ckID: 0
},