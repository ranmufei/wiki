### **请求接口**
index.php?app=Car&m=ClientInfoMobile&a=verification


### **公网测试**
http://www.apps.com/index.php?app=Car&m=ClientInfoMobile&a=verification&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| phone| 是 | string|电话号码 |  

### **返回结果**



    0 不存在

array 已存在返回客户、销售顾问信息  
      
      name  客户姓名   sale_name 销售顾问姓名



