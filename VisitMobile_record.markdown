### **请求接口**
index.php?app=Car&m=VisitMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=VisitMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| qday| 否 |   与今日相差天数，默认0，即当天|
| expect     | 否 |   0 需要回访客户 1 逾期未回访客户   |
| perPages     | 否 |   每页显示条数，默认10   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|number|-------   |int  |客户数量  |
|count| -------     |int    |客户总数     |
|client_id| -------     |int    |客户id     |
|content| -------     |string   |回访内容   |
|name| -------     |string    |客户姓名     |
|orginal_status| -------     |int    |客户状态     |
|phone| -------     |string    |手机号码     |
|plan_date| -------     |string   |计划回访日期     |
|deal_date| -------     |string   |成交日期    |
|pcarry_date| -------     |string   |计划提车日期   |