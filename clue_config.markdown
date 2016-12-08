### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=getSystemConfig



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=getSystemConfig&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
|type|否|2 是否启用维修项目  3 是否启用订单类型  4 预计完成时间是否允许修改 5 标签是否必填|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|fid_config   |--------    |array |订单类型列表  |
|fid_status  |--------    |int|0 不启用订单类型 1 启用订单类型 |
|label_status  |--------    |int |0 标签不必填 1 标签必填  |
| pro_status  |--------    |int |0 启用维修项目 1 不启用维修项目  |
| time_status|--------    |int |0 预计完成时间可修改 1 预计完成时间不可修改  |