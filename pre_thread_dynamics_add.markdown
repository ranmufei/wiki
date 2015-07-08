### **新增线索动态**
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=submit_dynamics

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
|remark      |动态内容 | string | `*`         |
|location    |坐标|string  | `*` |
|area        | 地区 | string | `*` |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


