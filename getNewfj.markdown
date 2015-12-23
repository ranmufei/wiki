### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=getNewfj
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=getNewfj&pid=97&cid=1
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |

### **示例**
````php

{
count: "7",
totalPages: 1,
nowPage: 1,
html: "<ul><li> &nbsp;&nbsp;NUM:7 1/1 页</li></ul>",
data: [
{
id: "510",
uid: "1",
cid: "1",
proid: "97",
tid: "0",
testid: "0",
ndid: "0",
serverid: "0",
time: "1442991392",
pic_url: "./Uploads/2015/0923/14/56024d2068c33.png",
key: "",
name: "F21DA1EA7E86F062FFC222985C90E56E1BC.png",
type: "image/png",
size: "133252",
extension: "png",
savepath: "2015/0923/14/",
savename: "56024d2068c33.png",
hash: "2c644ecbd709c06dfe4d9b7ecc5ee681",
download: "http://www.apps.com/index.php?app=Home&m=Visitor&a=download&val=4557"
},