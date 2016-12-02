### **请求接口**
index.php?app=AfterSalers&m=ClueMobile&a=getClueDetails



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=ClueMobile&a=getClueDetails&id=231&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   线索id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| goods|  | array  |维修单下产品详情（完全和报修线索一样的接口呀，显示什么自己取舍吧）|
| show|  | array  |线索详情|
| relateSup|  | array  |物料单详情（这里我不表态，还有已完成里有个物流动态，没必要显示吧）|