### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=add_revert
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=add_revert
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| proid| 是 |  项目的id  |
| uid| 是 | 登录人的id  |
| nid| 是 |  回复信息的id  |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status          |-------   |int    |1.设置成功，2.设置失败  |
|why| -------     |varchar  |1.设置成功，2.设置失败      |

