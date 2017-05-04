### **请求接口**
index.php?app=AfterSalers&m=SeaClueMobile&a=getClueDetails



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=SeaClueMobile&a=getClueDetails&id=231&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   线索id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| goods|  | array  |维修单下产品详情|
| show|  | array  |线索详情|
| relateSup|  | array  |物料单详情（在报修线索这可以不显示，因为这里根本就不可能会有这个）|