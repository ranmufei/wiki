### **请求接口**
index.php?app=AfterSalers&m=MyFxdMobile&a=setReFen



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=MyFxdMobile&a=setReFen&access_token=

### **请求方式**
POST


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   维修单id|
| pro| 是 |   array  （参数：id 维修id or 维修次序 pro_id 维修项目id name 项目名称 uid 维修人员）|
| pro_opt| 是 |   维修意见|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
0 失败 1 成功