### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=checkOrder

### **接口说明**
`订单详细信息`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=checkOrder

### **需要的参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type|  0/1            |int|0收款 1是付款         |
|o_type|              |int    | 判断是否为网络订单审核  0是本地订单审核  1为网络订单审核 |
|orderid|              |int    | 需要审核订单的id |
|revent|              |int    | 备注 |
 

### **其他参数**
无