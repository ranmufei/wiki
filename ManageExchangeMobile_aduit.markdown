### **请求接口**
index.php?app=Car&m=ManageExchangeMobile&a=aduit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageExchangeMobile&a=aduit

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| id| 是 | int|退换车id|
| type| 是 | int|1 同意  2 驳回|
| owner_id| 是 | int|车主id|
| addexchangecar| 是 | array|审核说明|
| car_id| 是 | int|车辆id|
| exchange_type| 是 | int|6：换车申请 7：退车申请|

     addexchangecar array  审核说明

               aduit_explain:'',

     return    1 添加成功