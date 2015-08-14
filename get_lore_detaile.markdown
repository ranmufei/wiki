### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getStorehouseDetailed

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getStorehouseDetailed

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   知识唯一ID   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int |int |知识唯一ID         |
|uid      |int         |int  |分享人ID    |
|category_id      |int         |int  |知识分类ID    |
|add_time      |int         |int  |分享知识时间    |
|edit_time      |int         |int  |修改知识时间    |
|edit_uid      |int         |int  |修改人ID    |
|share      |int         |int  |是否分享    |
|title      |string         |string  |知识标题    |
|titlepinying      |string         |string  |知识标题拼音码    |
|content      |string         |string  |知识内容    |
|label_id      |int         |int  |标签ID    |
|nice_count      |int         |int  |点赞数    |
|comment_count      |int         |int  |评论数    |
|like_count      |int         |int  |关注数    |
|down_id      |int         |int  |附件ID    |
|u_name      |string         |string  |分享人名称    |
|category_name      |string         |string  |分类 名称    |
| --------- |--------      |--------|--------       |
|comment      |array         |array  |评论树    |

