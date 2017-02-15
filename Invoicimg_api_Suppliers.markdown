### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=getSuppliersList

### **接口说明**
`分页`

### **请求方式**
get
### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getSuppliersList

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|str       |              |string  |搜索内容（产品名或者简码）|
|jump       |              |int    | 每页显示的条数  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript
{
count: "98",
totalPages: 7,
nowPage: 5,
data: [
{
id: "41",
pro_id: null,
sup_company: "测试22",
sup_code: "",
sup_phone: "84651123",
url: "www.kjl.com",
facsimile: "846521365",
email: "fsda@qq.com",
mark: "无",
creat_time: "2016-01-26 10:13",
uid: "1",
address: "fsfdsa",
isDelete: "0",
cid: "0",
default5: "0",
sup_level_id: "0",
username: "庆丰包子",
sup_level_name: "--"
},