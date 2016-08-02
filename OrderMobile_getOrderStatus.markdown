### **请求接口**
index.php?app=Car&m=OrderMobile&a=getOrderStatus



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=getOrderStatus
### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| order_id     | 是 |   订单id   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|visit|-------   |array  |回访人列表  |
|content|-------   |array  |回访内容列表  |
|method|-------   |array  |身份证类型  |
|pay|-------   |array  |支付方式  |
| ---------  |--------    |-------- |--------  |
|order|-------   |array  |订单信息：具体参数如下  |
| ---------  |--------    |-------- |--------  |
|name|-------   |string  |客户姓名  |
|phone|-------   |string  |电话号码  |
|sex|-------   |int  |性别  |
|birthday|-------   |string  |生日  |
|contacts|-------   |string  |订单联系人  |
|client_id|-------   |int  |客户id  |
|id|-------   |int  |订单id  |
|certificate_type|-------   |int|证件类型  |
|certificate_code|-------   |int|证件编号  |