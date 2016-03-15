### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_order

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order&status=2&type=2&access_token=e133ac84d35628422ca6c2c408667a&p=1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type       | 默认值2   |string |出库|
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
proList: [
{
ckID: "*",
subTypeId: "278",
maxhidden: false,
minhidden: false,
param0: "大",
param1: "10",
num: "90.00",
format: "FG_-D-10_0"
},
{
ckID: "*",
subTypeId: "279",
maxhidden: false,
minhidden: false,
param0: "小",
param1: "10",
num: "81.00",
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