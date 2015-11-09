### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=project_task_list



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=project_task_list&pid=120&uid=1&cid=1

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |
| uid| 是 |  使用人的id   |

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
count: "3",
totalPages: 1,
nowPage: 1,
html: "<ul><li> &nbsp;&nbsp;NUM:3 1/1 页</li></ul>",
data: [
{
tid: "78",
uid: "庆丰包子",
cid: "1",
pid: "120",
title: "测试任务三",
content: "范德萨范德萨",
time: "2015-09-24",
display: "0",
user: "6",
endtime: "2015-10-01",
status: "0",
leader: "1",
from: "0",
att: null,
mark: "",
uidd: "1",
plan: -1,
my_task: false,
permission: true,
permission_set: false,
user_list: [
{
img: "./Uploads/avatar/0/6.jpg",
name: "谷歌",
info: {
uid: "6",
username: "google",
name: "谷歌",
password: "",
email: "643788871@qq.com",
cid: "1",
zid: "357",
jid: "225",
age: "23",
phone: "15351",
mobile: "2351325",
area: "22",
spelling: "",
abbreviation: "",
update_time: "0"
},
jid: "公关"
}
]
},
{
tid: "77",
uid: "庆丰包子",
cid: "1",
pid: "120",
title: "测试任务二",
content: "范德萨范德萨",
time: "2015-09-24",
display: "0",
user: "344",
endtime: "2015-10-01",
status: "0",
leader: "1",
from: "0",
att: null,
mark: "",
uidd: "1",
plan: -1,
my_task: false,
permission: true,
permission_set: false,
user_list: [
{
img: "./Uploads/avatar/default.gif",
name: "冉帅1",
info: {
uid: "344",
username: "raneweshuai0010",
name: "冉帅1",
password: "",
email: "23654874@ewerwer.com",
cid: "1",
zid: "0",
jid: "0",
age: "0",
phone: "",
mobile: "15827451452",
area: "0",
spelling: "",
abbreviation: "",
update_time: "1447036032"
},
jid: null
}
]
},
{
tid: "76",
uid: "庆丰包子",
cid: "1",
pid: "120",
title: "测试测试",
content: "范德萨发大事",
time: "2015-09-24",
display: "1",
user: "350",
endtime: "2015-10-01",
status: "0",
leader: "1",
from: "0",
att: null,
mark: "",
uidd: "1",
plan: -1,
my_task: false,
permission: false,
permission_set: false,
user_list: [
{
img: "./Uploads/avatar/default.gif",
name: "小薇",
info: {
uid: "350",
username: "clp001",
name: "小薇",
password: "",
email: "16002120@qq.com",
cid: "1",
zid: "0",
jid: "0",
age: "0",
phone: "",
mobile: "13624556231",
area: "0",
spelling: "",
abbreviation: "",
update_time: "1447036032"
},
jid: null
}
]
}
]
}