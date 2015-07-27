# 添加日程
## 请求接口 

> /index.php?app=Calendar2&m=CalendarApi&a=Calendar_add

>  method : post

> *测试http://www.apps.com/index.php?app=Calendar2&m=CalendarApi&a=Calendar_add

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
|uid         |客户ID|int|    *|
|type      |日程标题 | int|0个人日程 1 工作日程 2 工作计划|
|important|日程优先级 | int |[选择优先级分类](http://192.168.1.240/ranmufei/apps/wikis/Calendar_category) | `*`|
|startime   |开始时间|string  | `*` |
|endtime   |开始时间|string  | `*` |
|tixintime  | 提醒时间 | int | 以分钟计 |
|actor      | 参与者(先不写吧) | array | |
|title      |日程标题 | string | `*`         |
|content    | 内容 | string | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |
