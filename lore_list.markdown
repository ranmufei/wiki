### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| p     | 是 |   当前页数   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int         |int |知识唯一ID         |
|uid       |string         |str  |知识分享人    |
|category_id       |int         |int  |知识分类ID    |
|add_time       |int         |int  |分享知识时间    |
|edit_time       |int         |int  |知识修改时间    |
|title       |string         |string  |知识标题    |
|titlepinyin       |string         |string  |标题拼音码    |
|label_id       |array         |array  |标签数组集    |
|nice_count       |int         |int  |点赞数    |
|comment_count       |int         |int  |评论数    |
|like_count       |int         |int  |关注数    |
|down_id       |int         |int  |附件ID    |


