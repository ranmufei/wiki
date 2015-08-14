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
|status     |success/error |string |请求状态         |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|errorDesc  |              |String |错误信息         |
|uid        |              |string |用户id           |
|cid        |              |String |用户所在的公司id  |
|domain     |              |String |用户所在的公司网址 |

