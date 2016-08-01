### **请求接口**
index.php?app=Car&m=ManageOrderMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageOrderMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| perPages     | 否 |   每页显示条数，默认10   |
| status     | 否 |   1 显示全部   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|name| -------     |string    |客户姓名     |
|status| -------     |string    |订单状态     |
|phone| -------     |string    |手机号码     |
|source| -------     |string   |客户来源     |
|earnest_money| -------     |float  |订金    |
|createtime| -------     |string    |订单时间     |
|intention_id| -------     |string    |车型     |
|type| -------     |string    |订单类型    |
|nsale_id| -------     |string    |销售顾问    |