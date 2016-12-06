### **请求接口**
index.php?app=AfterSalers&m=MyFxdMobile&a=getFxdDetails



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=MyFxdMobile&a=getRxdFcDetails&id=531&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   维修单id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| goods|  | array  |维修单下产品详情|
| show|  | array  |维修单详情|
| relateSup|  | array  |物料单详情|