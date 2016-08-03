### **请求接口**
index.php?app=Car&m=OrderMobile&a=setdownAduit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=setdownAduit

### **请求方式**
post

### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| id| 是 | int|订单id|
| client_id| 是 | int|客户id|
| downaduit| 是 | array|退单说明|

     downaduit array 退单信息
                  
                apply_explain:'',  退单说明

     return  0 添加失败      1 添加成功