### **请求接口**
/index.php?app=Asset&m=AsserApi&a=save_reject



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=save_reject

### **请求参数**

| 参数名称  |必填|     说明    |
|------|-----|------|
| id      | 是 |  申请id  |
| remark| 是 |  驳回的备注信息  |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|info|1.驳回成功 2.驳回失败    |string    |申请状态信息返还   |
|statu| “1”：成功，“0”：失败  |varchar  |申请状态标识返还      |