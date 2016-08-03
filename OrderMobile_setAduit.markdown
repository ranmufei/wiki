### **请求接口**
index.php?app=Car&m=TOrderMobile&a=setAduit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=setAduit

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| updateclient| 是 | array|客户信息|
| id| 是 | int|订单id|
| client_id| 是 | int|客户id|
| brand_id| 是 | int|意向车辆|
| product_id| 是 | int|车型号|
| format| 是 | array|车辆属性|
| updateorder| 是 | array|订单信息|
| addaduit| 是 | array|审核信息|

     updatetrack array 本次跟进信息
                  
                 track_aim:0,     跟进目的
                 track_method:0,  跟进方式
                 track_result:14, 跟进结果/默认14
                 new_level:0,     跟进级别
                 track_record:'', 跟进理由

     addtrack  array  下次跟进信息

                 track_aim,     跟进目的
                 track_method,  跟进方式
                 plan_date,     计划时间
                 track_reason,  跟进原因

     adddefeat array 战败信息
                 
                 reason int              战败原因
                 defeat_explain  string  战败说明
     return  0 添加失败      1 添加成功      2 添加战败失败