### **请求接口**
index.php?app=Car&m=ManageExchangeMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageExchangeMobile&a=record

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
|submit_date| -------     |string    |提交日期     |
|phone| -------     |string    |手机号码     |
|type| -------     |string   |退换车类型     |
|sastatus| -------     |float  |审核状态    |
|apply_explain| -------     |string    |申请说明     |
|nsale_id| -------     |string    |销售顾问    |