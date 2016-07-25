### **请求接口**
index.php?app=Pmanager&m=PmanegerApi&a=Notice_list



### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=Notice_list

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|nid|-------   |int    |动态id  |
|uid| -------     |int    |发布人id      |
|cid| -------     |int    |公司id      |
|display| -------     |int    |是否是隐私     |
|notice| -------     |int    |动态的内容      |
|pro_id| -------     |int    |所属项目     |
|test_id| -------     |int    |所属测试id      |
|server_id| -------     |int    |所属服务id    |
|task_id| -------     |int    |讨论id    |
|attic| -------     |int    |所属附件    |
|img| -------     |int    |用户图像地址  |
### **示例**
````php
{
nid: "671",
uid: "庆丰包子",
cid: "1",
display: "0",
notice: "的的d",
time: "08-11 15:14",
need_id: "0",
home_id: "0",
pro_id: "测试测试",
test_id: "64",
server_id: "0",
task_id: "71",
top: "2",
upid: null,
attic: null,
img: "./Uploads/avatar/0/1.jpg",
my: true
},