### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=add_user_project
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=add_user_project

### **请求字段**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|user|-------   |array| 参与项目的人员  |
|proid|-------   |int    | 项目id  |
|cid|-------   |int    |公司id  |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    |0.不是项目负责人 1.成功添加 3.添加失败 4. 最多添加25个人 5. 添加人员已经在团队中 6.项目负责人已在项目中|




