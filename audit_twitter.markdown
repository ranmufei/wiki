### **请求接口**
/index.php?app=Home&mAddTwitterApi&a=index

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |
| cid     | 是 |   公司id   |
| title     | 是 |  消息标题  |
| content     | 是 |   消息内容 |
| is_back     | 是 |   0不需要/1需要 是否需要回执 |
| info     | 是 |   @param $info:{uid:[],  //用户uid 数组     jid:[],  // 部门jid  数组     zid:[],  // 职位zid 数组     all:0   // 全公司
                } |



返回true或者1成功   false或者0失败