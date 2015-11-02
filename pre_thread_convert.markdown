### **转为客户**
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=convert

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
|id         |线索ID|string|    *|
|custom_company     |客户名称 | string | `*`         |
|custom_type |客户分类|string  | 选择 | * |
|trend  | 值=1 将动态也转给客户 | boolean | 默认选择 |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |

