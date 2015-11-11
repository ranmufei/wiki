### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=delete_pro
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=delete_pro

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   项目的id   |
| uid| 是 |  使用人的id   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|statu          |-------   |int    | 删除转态id  |
|why| -------     |varchar  |删除的状态文字说明      |



