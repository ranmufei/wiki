### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=project_serve_list



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=project_serve_list&pid=120&uid=1&cid=1

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
count: "2",
totalPages: 1,
nowPage: 1,
html: "<ul><li> &nbsp;&nbsp;NUM:2 1/1 页</li></ul>",
data: [
{
sid: "18",
uid: "1",
cid: "1",
pid: "120",
title: "测试服务2",
content: "123456+",
time: "2015-11-09",
user: "341",
endtime: "2015-11-29",
display: "0",
status: "0",
leader: "1",
att: null,
mark: "",
plan: 0,
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
sid: "17",
uid: "1",
cid: "1",
pid: "120",
title: "测试服务",
content: "测试测试",
time: "2015-11-09",
user: "341",
endtime: "2015-11-27",
display: "0",
status: "0",
leader: "1",
att: null,
mark: "",
plan: 0,
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
}
]
}