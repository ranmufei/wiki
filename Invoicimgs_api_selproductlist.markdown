### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getProContentList

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=getProContentList&access_token=dda0439fd69c3ad9316f6c2f2a0c36

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|code       |              |string |搜索内容（原料名或者简码）|
|cate       |              |int    | 点击分类查看所属产品  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript
{
count: "132",
totalPages: 6,
nowPage: 1,
data: [
{
id: "146", //原料id
name: "JXLQ",// 原料编码
class_id: "1",
y_code: "JXLQ", //原料编码
cat_id: "132", 
purchasePrice: "45.00", //采购价
cate_name: "原料", //分类名
supname: "机箱里卡", // 原料名
num: "571.00", // 库存数量
unitarr: [
{
id: "140", //单位id
unitid: "43", 
relation: "1", // 换算关系
unitname: "毫米" //单位名称
}
],
intonum: 1
},