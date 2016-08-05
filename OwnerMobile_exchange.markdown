### **请求接口**
index.php?app=Car&m=OwnerMobile&a=exchange



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OwnerMobile&a=exchange

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| id| 是 | int|车主id|
| car_vin| 是 | int|车辆VIN|
| car_id| 是 | int|车辆id|
| addbackcar| 是 | array|退换车信息|

     addbackcar array  退换车信息

                 exchange_type:6,    退换车类型
                 apply_explain:'',   申请说明

     return  0 添加失败      1 添加成功