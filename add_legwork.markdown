### **添加**

### **请求接口**
/index.php?app=Customer&m=MLegwork&a=add_legwork

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MLegwork&a=add_legwork&access_token=




### **添加字段**
|字段       |必填            |类型     |说明       |
| --------- |--------      |-------- |--------   |   
|gsy_id     |              |int      | 客户id    |
|contacts_id|              | int     | 联系人id   |
|address    |  *           | string  | 签到的地址 |
|lng        |  *           | string  |经度       |
|lat        |  *           | string  | 维度      |
|mark       |              | string  | 备注      |
|type       |              | int  | 0为客户1为线索2为汽车客户 ,如果选择了线索和汽车客户就不能选联系人      |
|file       |            |      |上传的附件|

### **添加字段**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |