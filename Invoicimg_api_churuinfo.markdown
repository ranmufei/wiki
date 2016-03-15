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
|info   |         | object |订单基本信息|
|info['list']   |     | array |订单产品信息|

|log|         | array | 操作日志 |
|storn|       | array | 仓库详细 |
|batchlist|       | array | 入库批次 |
``` javascript
