## 获取线索动态列表
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=view_dynamics

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrethread&a=view_dynamics&id=

### **公共参数** 
无

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|cname     |客户名称 | string | `*`         |
|contact   |联系人名称|string  | `*` |
|depart    | 部门 | string | |
|post      | 职务 | string | |
|mobile    | 手机 | string | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |

>数据结构
>>树
>>>二叉树
>>>>平衡二叉树
>>>>>满二叉树
