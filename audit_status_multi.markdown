# **更改多条审核/消息的状态**


### **请求接口**
/index.php?app=Home&m=AuditApi&a=changeStatusMulti


### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |
| cid     | 是 |   公司id   |
| id     | 是 |   审核的数据id , 必须填写数组  id[0] = 1 , id[1] = 2 之类的格式  |
| status     | 是 |   消息状态 ( 0未读 ，1已读 ，2已审核  |