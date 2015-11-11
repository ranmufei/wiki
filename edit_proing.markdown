### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=edit_proing
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=edit_proing
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| pid| 是 |  项目的id   |
| uid| 是 |  使用人的id   |
| pro_name| 是 |  项目名称  |
| objective| 是 |  项目目标   |
| end_time| 是 |  项目的结束时间  |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|statu          |-------   |int    | 修改后返还修改状态的信息 |
|info| -------     |varchar  |返还信息的文字说明     |


