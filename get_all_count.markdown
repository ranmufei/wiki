### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=get_all_count



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=get_all_count

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| uid| 是 |  登录人的id  |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|notice|-------   |int    | 动态树 |
|my_project|-------   |int    | 项目数  |
|my_task|-------   |int    | 任务数  |
|my_test|-------   |int    | 测试数  |
|my_serve|-------   |int    | 服务数  |


### **示例**
````php
{
notice: "573",
my_project: "84",
my_task: 79,
my_test: 29,
my_serve: 7
}