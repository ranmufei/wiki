### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=get_user



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=get_user&pid=120

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目id   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|user_list|-------   |int    |  项目成员|
