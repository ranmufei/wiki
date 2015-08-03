# 日程回复
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=answer

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=answer

### **接口说明**

### **请求方式**
post

### **浏览器查看**
无

### **公共参数** 
无

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id        |日程id|
|uid         |客户ID|int|    *|
|answerid         |被回复人的id|int|    *|
|comment      |回复内容 | varchar|*|


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |1 成功 / 0 失败 |string |返回结果         |
|info       | '' | string | 接口状态说明  |
