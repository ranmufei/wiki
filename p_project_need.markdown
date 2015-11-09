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
|uid|-------   |int    | 发布人的id  |
|title| -------     |varchar  |项目名称   |
|endtime|-------     |varchar   |结束时间|
|content| -------     |   varchar        |  任务说明    |

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