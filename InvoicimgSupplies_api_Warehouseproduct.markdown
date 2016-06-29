### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=instock_product_list

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
/http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=instock_product_list&access_token=

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|ckID      |              |string |根据仓库查询仓库产品库存|
|str        |              |string | 检索字段  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript
data:[
{
id: "92", //原料id
name: "34343", //原料名
ckID: 0,  //仓库id
num: "899.00" // 仓库数量
},
{
id: "91",
name: "新建物料",
ckID: 0,
num: "1000.00"
},
{
id: "90",
name: "测试测试",
ckID: 0,
num: "1000.00"
}
],
count: 66,
totalPages: 3