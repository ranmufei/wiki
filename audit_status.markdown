# **更改1条审核/消息的状态**


### **请求接口**
/index.php?app=Home&m=AuditApi&a=changeStatus


### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |
| cid     | 是 |   公司id   |
| id     | 是 |   审核的数据id  |
| is_read     | 是 |   消息状态 ( 0未读 ，1已读 ，2已审核  |


返回   true或者1成功   false或者0失败