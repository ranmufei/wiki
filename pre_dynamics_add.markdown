### **新增动态**
### **请求接口**
/index.php?app=Customer&m=MDynamic&a=add

/index.php?app=Customer&m=MDynamic&a=del&id=
(只需id 、get)

/index.php?app=Customer&m=MDynamic&a=del_schedule&id=(只需id 、get)(日程的删除)

/index.php?app=Customer&m=MDynamic&a=share_del&id=(只需id 、get)(详情页中删除共享记录和联合跟进人)

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
|id|关联的数据ID|string| `*` |
|type|关联的数据模块 `custom`客户动态; `thread`线索动态;`contacts`为联系人;`chance`机会 |string|`*`|
|remark      |动态内容 | string | `*`         |
|location    |坐标|string  | `*` |
|area        | 地区 | string | `*` |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


