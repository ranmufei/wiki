### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getProSupplies

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getProSupplies&access_token=dda0439fd69c3ad9316f6c2f2a0c36

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|name       |              |string |搜索内容（供应商名字）|
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript
{
count: "24",
totalPages: 1,
nowPage: 1,
data: [
{
id: "24",//供应商id
sup_company: "武汉在线科技" //供应商名字
},