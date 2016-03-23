### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_product_info

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
产品基本信息出入库信息 http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_product_info&productid=135&access_token=e133ac84d35628422ca6c2c408667a&p=1


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|proList    |         | array |基本信息数组 |
|tableHeader|         | object | 产品规格 |
|infos|         | object | 产品/仓库 |
|log|         | array | 产品出入库流水 |


### **浏览器查看**
全部仓库信息 http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_prock_info&productid=135&access_token=e133ac84d35628422ca6c2c408667a


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|storn|       | array | 仓库详细 |


### **浏览器查看**
批次信息 http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_probatchlist_info&productid=135&access_token=e133ac84d35628422ca6c2c408667a


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