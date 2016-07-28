### **请求接口**
index.php?app=Car&m=OwnerMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OwnerMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| expect     | 否 |   0 未提车 1 退换车   |
| perPages     | 否 |   每页显示条数，默认10   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|number|-------   |int  |客户数量  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|name| -------     |string    |车主姓名     |
|sstatus| -------     |string    |状态     |
|deal_date| -------     |string    |成交日期    |
|plan_date| -------     |string   |下次回访日期    |
|phone| -------     |string   |联系电话    |