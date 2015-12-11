### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=taskview



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=taskview

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目id   |
| tid| 是 |  任务的id  |
| uid| 是 |  登录人的id  |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|chatlist|-------   |int    | 动态列表 |
|count|-------   |int    | 动态的数量  |