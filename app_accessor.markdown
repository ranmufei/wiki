### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=app_accessor

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=app_accessor

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid  |  是 |   用户id   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|name   |              |string|菜单名称，应用附件|
|access|              |int |0=无权限，1=有权限|
### 实例

``` javascript
{"name":"\u5e94\u7528\u9644\u4ef6","access":1}