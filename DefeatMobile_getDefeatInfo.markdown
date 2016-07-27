### **请求接口**
index.php?app=Car&m=DefeatMobile&a=getDefeatInfo



### **公网测试**
http://www.apps.com/index.php?app=Car&m=DefeatMobile&a=getDefeatInfo

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| expect     | 是 |   0 待处理 1 已处理   |
| id     | 是 |   战败id   |
| client_id     | 是 |   客户id  |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|number|-------   |int  |客户数量  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|client_level| -------     |string   |客户级别    |
|name| -------     |string    |客户姓名     |
|orginal_status| -------     |int    |客户状态     |
|status| -------     |string    |客户状态对应的值     |
|phone| -------     |string    |手机号码     |
|plan_date| -------     |string   |计划跟进日期     |
|source| -------     |string   |客户来源     |
|track_reason| -------     |string   |跟进理由    |