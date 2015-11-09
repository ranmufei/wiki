### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=project_test_list



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=project_test_list&pid=120&uid=1&cid=1

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
testid: "71",
uid: "6",
cid: "1",
pid: "120",
task_id: "78",
title: "删除测试测试121231321",
content: "",
time: "2015-09-24",
user: "341",
endtime: "2015-09-30",
display: "0",
status: "0",
leader: "6",
att: null,
mark: "",
task_title: "测试任务三",
plan: -1,
user_list: [
{
img: "./Uploads/avatar/default.gif",
name: "杀阡陌",
info: {
uid: "341",
username: "shaqianmo",
name: "杀阡陌",
password: "",
email: "asdmin@dasd.d",
cid: "1",
zid: "0",
jid: "0",
age: "0",
phone: "",
mobile: "15987451451",
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
testid: "70",
uid: "6",
cid: "1",
pid: "120",
task_id: "78",
title: "删除测试测试",
content: "",
time: "2015-09-24",
user: "341",
endtime: "2015-09-30",
display: "0",
status: "0",
leader: "6",
att: null,
mark: "",
task_title: "测试任务三",
plan: -1,
user_list: [
{
img: "./Uploads/avatar/default.gif",
name: "杀阡陌",
info: {
uid: "341",
username: "shaqianmo",
name: "杀阡陌",
password: "",
email: "asdmin@dasd.d",
cid: "1",
zid: "0",
jid: "0",
age: "0",
phone: "",
mobile: "15987451451",
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
testid: "69",
uid: "1",
cid: "1",
pid: "120",
task_id: "76",
title: "范德萨范德萨",
content: "方法双方都撒",
time: "2015-09-24",
user: "344",
endtime: "2015-09-30",
display: "0",
status: "0",
leader: "1",
att: null,
mark: "",
task_title: "测试测试",
plan: -1,
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
}
]
}