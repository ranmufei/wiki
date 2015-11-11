### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=creatProject

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=creatProject

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户的id   |
| cid | 是 |   公司的id |
| pro_name | 是 |   项目名称 |
| objective | 是 |   项目目标 |
| display | 否 |   是否是私有项目。0是公开。1是私有 |
| end_time| 是 |   结束时间（时间戳） |
| user| 是 |  项目参加人的id  格式为“,60,55,78,79,136,134,82,34,24,1,6”|


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu     |int |int |创建的状态   0、是创建失败。1、创建成功。       |
|why     |string |string |返还创建的文字信息 ：创建成功、创建失败     |


