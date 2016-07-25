### **请求接口**
index.php?app=Car&m=TrackMobile&a=record



### **公网测试**
http://www.apps.com/index.php?app=Car&m=TrackMobile&a=record

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| qday| 否 |   与今日相差天数，默认0即当天|
| expect     | 否 |   0 需要跟进客户 1 逾期未跟进客户   |
| perPages     | 否 |   每页显示条数，默认10   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|ctime|-------   |string   |日期  |
|number| -------     |int    |客户数量     |
|qday| -------     |int    |与今日相差天数     |
