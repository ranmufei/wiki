### **新增线索日程**
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=add_schedule

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
|id         |客户ID|string|    *|
|title      |日程标题 | string | `*`         |
|startime   |开始时间|string  | `*` |
|tixintime  | 提醒时间 | int | 以分钟计 |
|actor      | 参与者(先不写吧) | array | |
|content    | 内容 | string | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


