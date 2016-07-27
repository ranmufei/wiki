### **请求接口**
index.php?app=Car&m=DefetMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=DefetMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| expect     | 否 |   0 待处理 1 已处理   |
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
|process_time| -------     |string   |申请时间    |