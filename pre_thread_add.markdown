### **请求接口**
/index.php?app=Customer&m=MPrethread&a=add_thread

http://www.apps.com/index.php?app=Customer&m=MPrethread&a=custom_thread_source&access_token=2c3b84599fcee0081496d827912c4a //来源列表

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
|cname     |客户名称   |输入框 | | `*`         |
|contact   |联系人名称 |输入框 | | `*` |
|state     |跟进状态   |选项   |1-未处理 2-已联系 3-关闭 | |
|sex       |性别       |选项   |1-男 2-女 ||
|depart    |部门       |输入框 | | |
|post      |职务       |输入框 | | |
|mobile    |手机       |输入框 | | |
|phone     |电话       |输入框 | | |
|email     |电子邮件   |输入框 | | |
|weibo     |微博       |输入框 | | |
|area      |地区       |输入框 | | | 
|address   |地址       |输入框 | | |
|code      |邮政编码   |输入框 | | |
|source    |线索来源   |选项|1-广告 2-研讨会 3-搜索引擎 4-客户介绍 5-其他|||
|remark    |备注       |输入框| | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |


