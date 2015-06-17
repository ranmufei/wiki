### **请求接口**
/index.php?app=Asset&m=AsserApi&a=rent_apply



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=rent_apply

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id      | 是 |   申租品的id  |
| number_get| 是 |   要租的编号信息array  |
| remark| 是 |   备注信息   |
| borrowtime| 是 |  借走的时间   |
| returntime| 是 |   归还时间   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|info|-------     |string    |申请状态信息返还   |
|status| -------     |varchar  |申请状态标识返还      |