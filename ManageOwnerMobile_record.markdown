### **请求接口**
index.php?app=Car&m=ManageOwnerMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageOwnerMobile&a=record

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
|name| -------     |string    |车主姓名     |
|status| -------     |string    |状态     |
|deal_date| -------     |string    |成交日期    |
|nsale_id| -------     |string   |销售顾问   |
|phone| -------     |string   |联系电话    |