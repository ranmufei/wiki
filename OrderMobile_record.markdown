### **请求接口**
index.php?app=Car&m=OrderMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| expect     | 否 |   0 新建订单 1 待处理   |
| perPages     | 否 |   每页显示条数，默认10   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|number|-------   |int  |客户数量  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|client_level| -------     |string   |客户级别    |
|name| -------     |string    |客户姓名     |
|status| -------     |string    |订单状态     |
|phone| -------     |string    |手机号码     |
|plan_date| -------     |string   |下次跟进计划     |
|source| -------     |string   |客户来源     |
|earnest_money| -------     |float  |订金    |
|car_status| -------     |string    |配车状态    |
|createtime| -------     |string    |订单时间     |
|car_id| -------     |string    |车型     |