### **请求接口**
index.php?app=Car&m=DefeatMobile&a=adddefeat



### **公网测试**
http://www.apps.com/index.php?app=Car&m=DefeatMobile&a=adddefeat

### **请求方式**
post

### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| adddefeat| 是 | array|本次跟进信息|
| client_id| 是 | int|客户id|

     updatetrack array 本次跟进信息
                  
                reason:0,           战败原因
                defeat_explain:'',  战败列表

     return  0 添加失败      1 添加成功