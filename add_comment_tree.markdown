### **请求接口**
/index.php?app=Lore&m=LoreApi&a=operateComment

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=operateComment

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   知识唯一ID   |
| comment | 是 |   评论内容 |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int |int |评论唯一ID         |
|lore_id       |int         |int  |知识唯一ID    |
|uid       |int         |int  | 用户唯一ID    |
|uid_name       |string         |string  |用户名称    |
|uid_avatar       |string         |string  |用户头像地址    |
|add_time       |string         |string  |评论时间    |
|reply_uid       |int         |int  |父评论的用户ID    |
|reply_name       |string         |string  |父评论的用户名称    |
|parent_id       |int         |int  |父亲评论的ID    |
|content       |string         |string  |评论内容    |
|attr       |array         |array  |子评论    |
