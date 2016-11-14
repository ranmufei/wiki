### **判断是否有下属**

### **请求接口**
/index.php?app=Customer&m=MLegwork&a=getZhiweiLeader


### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MLegwork&a=getZhiweiLeader&access_token=


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string  |请求状态         |
|info       |   有下属 /没有下属   |string  |      |


``` javascript

{
info: "没有下属",                            
status: "error",                     
}


