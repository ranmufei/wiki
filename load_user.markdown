### **请求接口**
/index.php?app=Core&m=Mclient&a=sypLogin

### **请求方式**
post

### **开发测试**
http://kaifa.linksame.com/index.php?app=Core&m=Mclient&a=sypLogin

### **公网测试**
http://www.apps.com/index.php?app=Core&m=Mclient&a=sypLogin

### **请求参数**

| 参数名称  |必填|     说明      |
|:-         |----|  -:|
| user     | 是 |   用户登录名   |
| password | 是 |   用户登录密码 |


### **返回结果**
|字段 |  值| 类型 | 说明|
| :-------- |---| --: |---|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|-----|-----|-----|-----|
|errorDesc| |String|错误信息|
|uid|     |string|用户id|
|cid|     |String|用户所在的公司id|
|domain|  |String|用户所在的公司网址|


