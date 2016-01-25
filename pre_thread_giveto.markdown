## 转移给他人列表
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=giveto


/index.php?app=Customer&m=MPrecustom&a=giveto


/index.php?app=Customer&m=MPrecontacts&a=giveto


/index.php?app=Customer&m=MPrechance&a=giveto

### **请求方式**
post


### **其他参数**
|字段       |说明            |类型      |必填           |
| --------- |--------       |--------  |--------       |
|ids        |线索id         |          |`*`|
|uid        |选择转移人的id  |          |`*`|

### **返回结果**
|字段       |值                          |类型     |说明           |
| --------- |--------                    |--------|--------       |
|statu      |1/0                         |int     |返回结果         |
|info       |分派成功/分派失败     | string | 接口状态说明  |