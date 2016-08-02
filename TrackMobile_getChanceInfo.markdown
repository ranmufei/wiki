### **请求接口**
index.php?app=Car&m=TrackMobile&a=getChanceInfo



### **公网测试**
http://www.apps.com/index.php?app=Car&m=TrackMobile&a=getChanceInfo

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| orginal_status| 是 |   客户状态|
| client_id     | 是 |   客户id   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|aim|-------   |array  |跟进目的  |
|level|-------   |array  |客户级别  |
|method|-------   |array  |跟进方式  |
|defeatreason|-------   |array  |战败原因  |
|track_result|-------   |array  |跟进结果  |
| ---------  |--------    |-------- |--------  |
|track|-------   |array  |本次跟进信息：具体参数如下  |
| ---------  |--------    |-------- |--------  |
|plan_date|-------   |string  |计划时间  |
|date|-------   |string  |跟进时间  |
|track_aim|-------   |int  |跟进目的  |
|track_method|-------   |int  |跟进方式  |
|track_result|-------   |int  |跟进结果  |
|old_level|-------   |int  |客户级别  |
|id|-------   |int  |跟进表id  |
|track_result|-------   |string  |跟进结果  |