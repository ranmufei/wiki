### **请求接口**
/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=getStorehouseList

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| p     | 是 |   用户登录名   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id     |int         |int |知识唯一ID         |
|uid       |string         |str  |知识分享人    |
|category_id       |array         |array  |返回数据 数组    |
|add_time       |array         |array  |返回数据 数组    |
|edit_time       |array         |array  |返回数据 数组    |
|title       |array         |array  |返回数据 数组    |
|titlepinyin       |array         |array  |返回数据 数组    |
|label_id       |array         |array  |返回数据 数组    |
|nice_count       |array         |array  |返回数据 数组    |
|comment_count       |array         |array  |返回数据 数组    |
|like_count       |array         |array  |返回数据 数组    |
|down_id       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|errorDesc  |              |String |错误信息         |
|-----      |-----         |-----  |-----           |
|uid        |              |string |用户id           |
|cid        |              |String |用户所在的公司id  |
|domain     |              |String |用户所在的公司网址 |

