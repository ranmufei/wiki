### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=getBatchInfo

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
出库订单详情  http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=getBatchInfo&id=191&access_token=e133ac84d35628422ca6c2c408667a


### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id       |              |int |订单id|
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info   |         | object |订单基本信息|
|info['list']   |     | array |订单产品信息|
|log|         | array | 操作日志 |
|batchlist|       | array | 批次记录 |
|batchSarial|       | array | 序列号记录 |
|outStronOrder|       | array |出库单记录 |
``` javascript
