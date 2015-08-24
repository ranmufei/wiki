### **请求接口**
/index.php?app=Pmanager&m=&a=project_list
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=&a=project_list


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|number      | -------     |varchar  |物品编号      |
|type        | -------    |varchar  |目前未用      |
|already_num | -------     |int  |申租品已经借出数量     |
|ntime       |  -------   |varchar     |  购买时间   |
|names       |-------     |varchar   |物品名称          |
|old         |   -------         |varchar　　|　折旧率 |
|is_old| -------   |int　|　是否属于折旧     |
|num |    -------         |int | 物品数量 |
|remark|  -------      | varchar   |  备注信息   |
|gunit|   -------        |  varchar | 物品单位|
|cateid|   -------       |  int  |  大分类（1）易耗品（2）申租品（3）折旧品|
|buytime|  -------        | varchar    |  添加时间   |
|price|   -------          |   float |  物品单价    |
|now_tprice        | -------     | varchar   | 数量*单价后 折旧的价格   |
|img|  -------         |   varchar  |  物品图片地址    |
|cat|  -------         |   varchar  |  小分类名称   |


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