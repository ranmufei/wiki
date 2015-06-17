### **请求接口**
/index.php?app=Asset&m=AsserApi&a=pass_save



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=pass_save

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id      | 是 |  申请id  |
| uid| 是 |  当前用户的uid  |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|info|1.申请成功 2.申请失败    |string    |申请状态信息返还   |
|statu| “1”：成功，“3”：库存 不足，“0”：失败  |varchar  |申请状态标识返还      |