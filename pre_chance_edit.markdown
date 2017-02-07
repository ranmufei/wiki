### **修改销售机会**

### **请求接口**
/index.php?app=Customer&m=MPrechance&a=edit_chance

/index.php?app=Customer&m=MPrechance&a=delpro // 删除  参数（id )

/index.php?app=Customer&m=MPrechance&a=edit_chance  //修改  参数（id  num)

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
|name      |机会名称   |输入框 | | `*`         |
|custom_id |所属客户 |选择 |[查询客户](http://192.168.1.240/ranmufei/apps/wikis/pre_custom_search_like) | （不能修改） |
|count     |销售金额 |输入框 |||
|type      |机会类型 |选项 | 1-新客户机会 2-老客户机会 ||
|source    |机会来源 |选项 | 1-广告 2-研讨会 3-搜索引擎 4-客户介绍 5-其他 | |
|remark    |备注     |输入框| | |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |

