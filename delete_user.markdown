### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=delete_user
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=delete_user
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   要删除成员的id |
| pid     | 是 |   要删除成员对应项目的id |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status          |-------   |int    | 1：删除成功。2：删除失败。  |
|info| -------     | varchar |  删除状态的文字说明，解释同上。    |
