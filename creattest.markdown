### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=creattest



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=creattest

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目id   |
| uid| 是 |  创建人id  |
| endtime| 是 |  任务束时间  |
| user| 是 |  参与任务的人员 |
| display| 是 | 公开私密 |
| content| 是 |测试内容 |
| title| 是 | 测试名称 |
| taskid| 是 | 任务的id |
| leader| 是 | 项目负责人的id |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    | 1.创建成功 2.创建失败 |
|info|-------   |int    |  1.创建成功 2.创建失败  |