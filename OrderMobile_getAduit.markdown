### **请求接口**
index.php?app=Car&m=OrderMobile&a=getAduit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=getAduit

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   订单id|
| client_id     | 是 |   客户id   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|name|-------   |string  |客户姓名  |
|certificatetype| -------     |string    |证件类型     |
|orginal_status| -------     |string    |客户信息状态     |
|certificate_code| -------     |string   |客户编号    |
|number| -------     |string    |订单编号    |
|status| -------     |string    |订单状态     |
|type| -------     |string    |订单类型    |
|nsale_id| -------     |string   |销售顾问     |
|createtime| -------     |string   |创建时间    |
|order_contacts| -------     |string   |订单联系人    |
|contacts| -------     |string   |提车联系人    |
|car_contacts| -------     |string   |预计提车时间   |
|earnest_money| -------     |float   |订金  |