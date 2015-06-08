### **请求接口**
/index.php?app=Notice&m=NoticeApi&a=detailed_notice

### **请求方式**
get/post

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   公告id   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|title        |              |string |公告标题           |
|worktime     |              |String |开始时间 |
|outtime     |              |String |过期时间 |
|content     |              |String |公告详情 |
|name     |              |String |发布人 |
