### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=my_serve_list



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=my_serve_list&pid=120&uid=1&cid=1

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| p| 是 |  分页的当前页   |
| uid| 是 |  使用人的id   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|tid|-------   |int    | 任务id |
|title|-------   |int    | 任务标题  |
|content|-------   |int    | 内容 |
|display|-------   |int    | 是否私有|
|endtime|-------   |int    | 结束时间|
|content|-------   |int    | 内容 |
|uid|-------   |int    | 发布人的id  |
|title| -------     |varchar  |项目名称   |
|endtime|-------     |varchar   |结束时间|
|content| -------     |   varchar        |  任务说明    |



### **示例**
````php

list: {
count: 39,
data: [
{
tid: "87",
uid: "1",
cid: "1",
pid: "127",
title: "测试1111",
content: "范德萨范德萨发的萨芬撒",
time: "2015-11-14 11:45",
display: "0",
user: "341",
endtime: "2015-11-21 00:00",
status: "0",
leader: "1",
from: "0",
att: null,
mark: "",
uidName: "庆丰包子",
leaderName: "庆丰包子",
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
update_time: "1447209674"
},
jid: null
}
],
pro_name: "测试项目11112"
}
