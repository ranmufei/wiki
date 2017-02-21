### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=getAfterSalersInfo



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=getAfterSalersInfo&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| pageSize| 否 | 每页显示条数（默认10）   |
| search| 否 | 筛选内容（订单号、售后单号、客户姓名）   | 

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|f_id| -------     |string    |售后单号     |
|o_id| -------     |string    |订单号     |
|c_name| -------     |string   |客户名称    |
|num| -------     |int    |商品数量    |
|js_name| -------     |string    |经手人     |
|sh_name| -------     |string    |审核人     |
|sh_status| -------     |string    |审核状态     | 
|status| -------     |string    |状态     | 
|createtime| -------     |string    |创建时间     | 
|suctime| -------     |string    |完成时间     | 