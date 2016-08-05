### **请求接口**
index.php?app=Car&m=ManageExchangeMobile&a=getExchange



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageExchangeMobile&a=getExchange

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   退换车id  |  
| owner_id| 是 |   车主id  | 
| client_id| 是 |   客户id  | 

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|exchange|-------   |array  |退换车信息  |
|method|-------   |array  |跟进方式  |
