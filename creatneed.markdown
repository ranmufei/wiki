### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=creatneed



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=creatneed&pid=120&uid=1&cid=1

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目id   |
| uid| 是 |  创建人id  |
| endtime| 是 |  讨论结束时间  |
| user| 是 |  参与谈论的人员 |
| display| 是 | 公开私密 |
| content| 是 | 需求详细内容 |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    | 1.创建成功 2.创建失败 |
|info|-------   |int    |  1.创建成功 2.创建失败  |





