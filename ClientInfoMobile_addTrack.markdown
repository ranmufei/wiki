### **请求接口**
index.php?app=Car&m=ClientInfoMobile&a=addTrack



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ClientInfoMobile&a=addTrack

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| id| 是 | int|战败表id------无跟进计划（销售顾问）列表接口中获取|
| client_id| 是 | int|客户id------获取方式同上|
| plan_date| 是 | string|计划日期|
| track_aim| 是 | int|跟进目的|
| track_method| 是 | int|跟进方式|
| track_reason| 是 | int|跟进理由|

     return  0 添加失败      1 添加成功