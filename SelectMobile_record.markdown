### **请求接口**
index.php?app=Car&m=SelectMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=SelectMobile&a=record

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
|client_level| -------     |string   |客户级别    |
|name| -------     |string    |客户姓名     |
|orginal_status| -------     |int    |客户状态     |
|status| -------     |string    |客户状态对应的值     |
|phone| -------     |string    |手机号码     |
|time_cards| -------     |string   |建卡时间     |
|description| -------     |string   |建卡渠道    |
|plan_date| -------     |string   |下次跟进时间    |
|source| -------     |string   |来源    |
|intention_id| -------     |string   |意向品牌    |