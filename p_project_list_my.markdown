### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=project_list_my
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=project_list_my
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |
| uid| 是 |  使用人的id   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    | 项目id  |
|uid| -------     |varchar  |用户id      |
|pro_name| -------    |varchar  |项目名称   |
|objective| -------     |int  |项目目标    |
|time|  -------   |varchar     |  创建时间  |
|end_time|-------     |varchar   |项目结束时间        |
|leader|   -------         |varchar　　|　项目负责人id |
|user| -------   |int　|参加项目人员    |
|display|    -------         |int | 是否是私有项目，0为公开，1位私有|
|percent|  -------      | varchar   |  项目进度百分比  无‘%’，需要自己加|
| is_past | -------     | varchar   | 是否过期true过期  false没有过期|
|leaderinfo|  -------         |   varchar  |  负责人信息内容    |
|userinfo|  -------         |   varchar  |  参与人员信息内容   |


### **示例**
````php

list: [
{
id: "124",
uid: "1",
cid: "1",
pro_name: "轻轻去去去f",
objective: "的发生的方式",
time: "2015-11-10",
end_time: "1447689600",
leader: "1",
user: {
1: "367",
2: "360"
},
display: "0",
status: "0",
isOrder: "0",
percent: "20",
nd: "1",
tsk: "0",
tst: "0",
svr: "0",
dt: "2",
uidd: "1",
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
zid: "38",
jid: "37",
age: "601",
phone: "7535831",
mobile: "15827422",
area: "66",
spelling: "",
abbreviation: "",
update_time: "0"
},
jid: "行政部"
},
userinfo: [
{
img: "./Uploads/avatar/default.gif",
name: "funcks",
info: {
uid: "367",
username: "冉阿",
name: "funcks",
password: "",
email: "234233@qq.com",
cid: "1",
zid: "366",
jid: "3",
age: "0",
phone: "",
mobile: "15827145902",
area: "0",
spelling: "",
abbreviation: "",
update_time: "1447036032"
},
jid: null
},
{
img: "./Uploads/avatar/default.gif",
name: "黄飞鸿",
info: {
uid: "360",
username: "wangfeihong",
name: "黄飞鸿",
password: "",
email: "baidu@bai.com",
cid: "1",
zid: "3",
jid: "3",
age: "0",
phone: "",
mobile: "15725484512",
area: "0",
spelling: "",
abbreviation: "",
update_time: "1447036032"
},
jid: null
}
]
},