### **新增联系人**

### **请求接口**
/index.php?app=Customer&m=MPrecontacts&a=add_contacts

### **接口说明**

### **请求方式**
post

### **浏览器查看**
无

### **公共参数** 
无

### **其他参数**
|字段       |说明            |表单类型|表单补充    |必填           |
| --------- |--------      |--------|------- |--------       |
|name      |姓名   |输入框 | | `*`         |
|custom_id |所属客户 |选择 |[查询客户](http://192.168.1.240/ranmufei/apps/wikis/pre_custom_search_like) | |
|sex       |性别     |选项 |1-男 2-女 | |
|post      |职位     |输入框 |||
|depart    |部门     |输入框 | | |
|mobile    |手机     |输入框 | | |
|phone     |电话     |输入框 | | |
|email     |邮箱     |输入框 | | |
|birthday  |生日     |日期 | | |
|age       |年龄     |输入框 | | |
|address   |住址     |输入框 | | | 
|hometown  |家乡     |输入框 | | |
|remark    |备注     |输入框| | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


