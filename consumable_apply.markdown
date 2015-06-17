### **请求接口**
/index.php?app=Asset&m=AsserApi&a=consumable_apply



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=consumable_apply

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   所申请的物品id   |
| num    | 是 |   申请物品的数量   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    |申请的状态标识别  |
|info| -------     |varchar  | 申请的状态详细   |