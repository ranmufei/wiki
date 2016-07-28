### **请求接口**
index.php?app=Car&m=VisitMobile&a=getChanceInfo



### **公网测试**
http://www.apps.com/index.php?app=Car&m=VisitMobile&a=getChanceInfo

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| client_id     | 是 |   客户id   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|contnet|-------   |array  |回访内容  |
|plan|-------   |array  |回访计划  |
|satisfied|-------   |array  |满意度  |
|visit_id|-------   |array  |被回访人  |
| ---------  |--------    |-------- |--------  |
|visit|-------   |array  |本次回访信息：具体参数如下  |
| ---------  |--------    |-------- |--------  |
|plan_date|-------   |string  |计划时间  |
|date|-------   |string  |回访时间  |
|content|-------   |int  |回访内容  |
|plan|-------   |int  |回访计划  |
|visit_id|-------   |int  |被回访人  |
|id|-------   |int  |回访表id  |
|type|-------   |string  |回访类型  |