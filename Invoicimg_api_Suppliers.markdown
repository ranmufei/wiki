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
count: "26",
totalPages: 2,
nowPage: 1,
data: [
{
id: "60",
name: "sad",  //商品名
cate_id: "1",
brand: "",  //品牌
shelfLife: "0",  // 0表示没有保释期，1表示有保质期
cate_name: "数码545"  //分类名
},