### **请求接口**
/index.php?app=Notice&m=NoticeApi&a=notice_list

### **请求方式**
get/post

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| p | 否 |   分页码，若不填则默认第一页 |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id  |              |String |公告id         |
|title        |              |string |公告标题           |
|worktime        |              |String |公告开始时间  |
|name        |              |String |发布人  |

