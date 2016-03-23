### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=nextCheck

### **接口说明**
`提交下步审批`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=nextCheck

### **需要的参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|orderid|  ---           |int|订单的id      |
|revent|              |varchar    |备注  |
|chcek_id|              |int    | 提交的审批人  |
|uid|              |int    | 登录人的id  |
