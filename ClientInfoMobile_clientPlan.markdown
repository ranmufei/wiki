### **请求接口**
index.php?app=Car&m=ClientInfoMobile&a=clientPlan



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ClientInfoMobile&a=clientPlan

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| perPages     | 否 |   每页显示条数，默认10   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|level| -------     |string   |客户级别    |
|name| -------     |string    |客户姓名     |
|source| -------     |string    |客户来源     |
|description| -------     |string    |建卡渠道     |
|time_cards| -------     |string    |建卡时间     |