### **请求接口**
index.php?app=Car&m=ManageHvisitMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageHvisitMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| perPages     | 否 |   每页显示条数，默认10   |
| status     | 否 |   1 查询全部   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|name| -------     |string    |车主姓名     |
|orginal_status| -------     |int    |客户状态     |
|phone| -------     |string    |手机号码     |
|plan_date| -------     |string   |计划回访日期     |
|date| -------     |string   |回访日期     |
|type| -------     |string   |回访类型    |
|record| -------     |string   |回访记录   |
|nsale_id| -------     |string   |销售顾问   |