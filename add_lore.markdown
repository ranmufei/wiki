### **请求接口**
/index.php?app=Lore&m=LoreApi&a=addStorehouse

### **请求方式**
post

### **公网测试**
http://www.apps.com/index.php?app=Lore&m=LoreApi&a=addStorehouse

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| storeCategory     | 是 |   知识分类   |
| storeTitle | 是 |   知识标题 |
| storeTitlepinyin | 是 |   标题拼音码 |
| StoreContent | 是 |   知识内容 |
| storeShare | 否 |   配置为私有还是分享出去 |
| storeLabels| 是 |   所选择的标签ID |
| storeDown | 否 |   附件ID |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data     |array |array |成功返回新的知识列表（参考列表接口字段）         |


