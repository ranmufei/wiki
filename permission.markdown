### **请求接口**
/index.php?app=Asset&m=AsserApi&a=permission



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=permission

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   需要验证是否拥有审核物品权限的用户  |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
| ---------       |0   |int    |无权限   |
| ---------         |1   |int    |有权限  |