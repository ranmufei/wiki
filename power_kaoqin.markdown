## 考勤有审核权限的人员列表
### **请求接口**
/index.php?app=Home&m=Audit&a=select_auditlist

### **请求方式**
post

### **公共参数** 
````php
apps:Kaoqin
ms:Jilu
as:person_shenh
````
### **接口说明**




### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data       |array         |array  |请看下面代码 |


### **data 数组格式**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|uid       |         |interger  |人员uid |
|name       |         |string  |人员姓名 |
|zname       |         |string  |职位名称 |
|img       |         |string  |人员头像 |
