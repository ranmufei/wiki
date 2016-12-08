### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=getOrderData



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=getOrderData&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| p| 否 |   当前页码数|
| search| 否 |   查找条件|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| goods|  | array  |维修单下产品详情|
| show|  | array  |线索详情|
| relateSup|  | array  |物料单详情（在报修线索这可以不显示，因为这里根本就不可能会有这个）|