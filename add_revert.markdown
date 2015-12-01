### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=add_revert
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=add_revert
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| give_uid     | 是 |  回复给人员的id  |
| nid| 是 | 动态的id  |
| uid| 是 |  当前使用人的id   |
| notice| 是 |  回复的内容   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status          |-------   |int    |1.回复成功，2.回复失败  |
|info| -------     |varchar  |1.回复成功，2.回复失败      |
|data| -------     |varchar  |  返回的回复信息   |
