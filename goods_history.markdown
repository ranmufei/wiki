### **请求接口**
/index.php?app=Asset&m=AssetApi&a=goods_history



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=goods_history

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   项目的id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|time|-------   |int    |创建时间   |
|userid| -------     |varchar  |申请人姓名    |
|profj|-------     |varchar   |附件信息|
|user_list| -------     |   varchar        |  参与人员id   |
|userinfo| -------    |varchar  |参与人员详细信息|
|chatlist| -------     |int  |动态列表   |
|nid| -------     |int  |需求id    |
|uid| -------     |int  |用户id  |
|cid| -------     |int  |公司id  |
|display| -------     |int  |是否私有0公开  1私有  |
|time| -------     |int  |发布时间|
|need_id| -------     |int  |需求id  |
|pro_id| -------     |int  |所属项目id |
|img| -------     |int  |所属图片id|
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