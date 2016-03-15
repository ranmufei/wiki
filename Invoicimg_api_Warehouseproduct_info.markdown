### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_product_info

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
/http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_product_info&access_token=

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p          |              |string |分页         |
|ckid       |              |string |仓库id|
|productid  |              |string | 检索字段  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|proList    |         | array |基本信息数组 |
|tableHeader|         | object | 产品规格 |
|infos|         | object | 产品/仓库 |
|log|         | array | 产品出入库流水 |
|storn|       | array | 仓库详细 |
|batchlist|       | array | 入库批次 |
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