### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=task_editing
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=task_editing
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid| 是 |  登录人的id   |
| tid| 是 |  任务的id   |
| title| 是 |  编辑的标题   |
| content| 是 | 编辑的内容 |
| endtime| 是 | 编辑的结束时间  |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    |1.编辑成功。0.编辑失败  |
|info| -------     |varchar  |1.编辑成功。0.编辑失败   |