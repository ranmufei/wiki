### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=project_need



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=project_need&pid=97&cid=1

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|nid|-------   |int    |需求id   |
|cid| -------     |varchar  |公司id   |
|display|-------     |varchar   |是否私有 0不是 1是的|
|notice| -------     |   varchar        |  动态内容    |
|time| -------    |varchar  |发布时间|
|pro_id| -------     |int  |所属项目名称|
|task_id| -------     |int  |任务id   |
|img| -------     |int  |用户图像   |
|my| -------     |int  |是否属于自己发的消息true是  false不是   |
|top| -------     |int  |是否是谈论结果0不是讨论结果1是谈论结果  |


### **示例**
````php
{
list: [
{
nid: "660",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "范德萨发大水",
time: "07-25 16:00",
need_id: "47",
home_id: "0",
pro_id: "创建另一个项目测试",
test_id: "0",
server_id: "0",
task_id: "0",
top: "0",
upid: "",
attic: "",
img: "./Uploads/avatar/0/1.jpg",
my: true,
uidd: "1"
},
{
nid: "645",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "又4月又4月",
time: "07-23 18:11",
need_id: "47",
home_id: "0",
pro_id: "创建另一个项目测试",
test_id: "0",
server_id: "0",
task_id: "0",
top: "0",
upid: "",
attic: "",
img: "./Uploads/avatar/0/1.jpg",
my: true,
uidd: "1"
},
{
nid: "644",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "5要有又4月",
time: "07-23 18:10",
need_id: "47",
home_id: "0",
pro_id: "创建另一个项目测试",
test_id: "0",
server_id: "0",
task_id: "0",
top: "1",
upid: "",
attic: "",
img: "./Uploads/avatar/0/1.jpg",
my: true,
uidd: "1"
},
{
nid: "643",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "堣",
time: "07-23 18:10",
need_id: "47",
home_id: "0",
pro_id: "创建另一个项目测试",
test_id: "0",
server_id: "0",
task_id: "0",
top: "0",
upid: "",
attic: "",
img: "./Uploads/avatar/0/1.jpg",
my: true,
uidd: "1"
}
],
count: "4"
}