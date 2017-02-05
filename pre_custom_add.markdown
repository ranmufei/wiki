### **新增客户**

### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=add_custom

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
|custom_company|客户名称   |输入框 | | `*`         |
|custom_number|客户编码  |输入框 | |         |
|custom_type   |分类 |选择 |[选择客户分类](http://192.168.1.240/ranmufei/apps/wikis/pre_custom_type_list) | `*` |
|pid       |父客户   |选择 |[选择父级客户](http://192.168.1.240/ranmufei/apps/wikis/pre_custom_search_like) | |
|level     |重要级别   |选项   |1-A(重点客户) 2-B(普通客户) 3-C(非优先客户) ||
|url       |公司网址   |输入框 | | |
|company_phone |公司电话  |输入框 | | |
|facsimile |传真       |输入框 | | |
|email     |公司邮箱   |输入框 | | |
|scope     |员工人数   |输入框 | | |
|sales     |年销售额   |输入框 | | |
|custom_address |公司地址（用百度地图） | | | | 
|lng|经度（用百度地图） | | | | 
|lat|维度（用百度地图） ||| | 
|trade   |行业       |输入框 | | |
|remark    |备注       |输入框| | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


