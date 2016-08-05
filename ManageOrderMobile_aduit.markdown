### **请求接口**
index.php?app=Car&m=ManageOrderMobile&a=aduit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageOrderMobile&a=aduit

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| id| 是 | int|订单id|
| client_id| 是 | int|客户id|
| type| 是 | int|2驳回退单，3同意退单|
| audit_explain| 是 | string|审核说明|

     return  0 添加失败      1 添加成功