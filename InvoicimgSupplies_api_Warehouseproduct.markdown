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
