### **请求接口**
index.php?app=Eboss&m=EbossApi&a=promission



### **公网测试**
http://www.apps.com/index.php?app=Eboss&m=EbossApi&a=promission

### **请求接口**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|uid|-------   |int    |登录人员的uid|


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status|-------   |int    |权限的状态值1.有权限2.没有权限|
|info| -------     |int    |权限的状态值1.有权限2.没有权限     |


### **示例**
````php
{
status: 0,
info: "没有权限"
}