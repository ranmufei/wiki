### **请求接口**
/index.php?app=Pmanager&m=Procon&a=index



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=Procon&a=index&pid=97

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   物品id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|nid|-------   |int    |需求id   |
|uid| -------     |varchar  |用户id   |
|display|-------     |varchar   |是否私有 0不是 1是的|
|notice| -------     |   varchar        |  动态内容    |
|time| -------    |varchar  |发布时间|
|pro_id| -------     |int  |所属项目名称|
|task_id| -------     |int  |任务id   |
|img| -------     |int  |用户图像   |
|my| -------     |int  |是否属于自己发的消息true是  false不是   |

### **示例**
````php
{
nid: "661",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "范德萨发大水",
time: "07-25 16:00",
need_id: "0",
home_id: "0",
pro_id: "创建另一个项目测试",
test_id: "0",
server_id: "0",
task_id: "69",
top: "0",
upid: null,
attic: null,
img: "./Uploads/avatar/0/1.jpg",
my: true
},