### **请求接口**
/index.php?app=Barcode&m=PmanegerApi&a=project_list



### **公网测试**
http://www.apps.com/index.php?app=Barcode&m=PmanegerApi&a=project_listly

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|info|       |string    |申请状态信息返还   |
|status| "1":成功 "0":失败    |varchar  |申请状态标识返还      |


### **示例**
````php

{
id: "98",
uid: "1",
cid: "1",
pro_name: "测试测试",
objective: "测试目标",
time: "2015-08-11",
end_time: "1439827200",
leader: "1",
user: {
1: "350",
2: "1"
},
display: "0",
status: "0",
isOrder: "0",
percent: "100",
nd: "1",
tsk: "2",
tst: "1",
svr: "0",
dt: "3",
uidd: "1",
is_past: true,
leaderinfo: {
img: "./Uploads/avatar/0/1.jpg",
name: "庆丰包子",
info: {
uid: "1",
username: "sving",
name: "庆丰包子",
password: "",
email: "137283358@qq.com",
cid: "1",
zid: "4",
jid: "3",
age: "601",
phone: "7535831",
mobile: "15827422",
area: "66",
spelling: "",
abbreviation: "",
update_time: "0"
},
jid: "技术部"
},
userinfo: [
{
img: "./Uploads/avatar/0/350.jpg",
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
update_time: "1440399841"
},
jid: "技术部"
},
{
img: "./Uploads/avatar/0/1.jpg",
name: "庆丰包子",
info: {
uid: "1",
username: "sving",
name: "庆丰包子",
password: "",
email: "137283358@qq.com",
cid: "1",
zid: "4",
jid: "3",
age: "601",
phone: "7535831",
mobile: "15827422",
area: "66",
spelling: "",
abbreviation: "",
update_time: "0"
},
jid: "技术部"
}
]
},