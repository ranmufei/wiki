### **请求接口**
index.php?app=Car&m=ClientInfoMobile&a=addClient



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ClientInfoMobile&a=addClient

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| client| 是 | array|客户信息|
| reception| 是 | array|意向信息|

     client array 客户信息
                  
                 name               客户姓名
                 sex                性别  1 男  2女
                 phone              电话号码
                 source_id          客户来源id
                 certificate_type   证件类型
                 certificate_code   证件编号

     reception  array  意向信息

                     brand_id:'',                string     车辆id


     return  0 添加失败      1 添加成功 