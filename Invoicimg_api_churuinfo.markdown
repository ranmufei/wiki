### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=instock_order_info

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
出库订单详情  http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order_info&id=1470&type=0&access_token=e133ac84d35628422ca6c2c408667a&p=1

入库订单详情  http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=instock_order_info&id=1497&type=1&access_token=e133ac84d35628422ca6c2c408667a&p=1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id       |              |int |订单id|
|type  |              |string |  0 出库订单  1 入库订单|
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
