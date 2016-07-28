### **请求接口**
index.php?app=Car&m=ManageHtrackMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageHtrackMobile&a=record

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
|name| -------     |string    |客户姓名     |
|orginal_status| -------     |int    |客户状态     |
|phone| -------     |string    |手机号码     |
|plan_date| -------     |string   |计划跟进日期     |
|date| -------     |string   |实际跟进日期     |
|track_method| -------     |string   |跟进方式    |
|track_result| -------     |string   |跟进结果    |
|nsale_id| -------     |string   |销售顾问    |
|track_record| -------     |string   |跟进记录    |