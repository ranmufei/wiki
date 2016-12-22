### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=getFxdDetails



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=getFxdDetails&id=246&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   线索id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| goods|  | array  |维修单下产品详情（显示的数据和前面的都一样，可能这里比较重要吧）|
| show|  | array  |线索详情|
| relateSup|  | array  |物料单详情|