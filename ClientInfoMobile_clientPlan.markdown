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
|number|-------   |int  |客户数量  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|clientlevel| -------     |string   |客户级别    |
|name| -------     |string    |客户姓名     |
|reason| -------     |string    |主要原因     |
|sstatus| -------     |string    |处理动作     |
|process_opinion| -------     |string    |处理意见     |
|apply_time_time| -------     |string   |申请时间    |