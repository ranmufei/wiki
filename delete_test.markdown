### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=delete_test
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=delete_test
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| tid| 是 | 测试的id   |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    |1.删除成功 0.删除失败   |
|why| -------     |varchar  |1.删除成功 0.删除失败  |