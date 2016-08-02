### **请求接口**
index.php?app=Car&m=OrderMobile&a=setCar



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OrderMobile&a=setCar

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| updatetrack| 是 | array|本次跟进信息|
| addowner| 是 | array|车主信息|
| addvisit| 是 | array|回访信息|
| addcar| 是 | array|车辆信息|
| id| 是 | int|跟进表id|
| client_id| 是 | int|客户id|
| orderid| 是 | int|订单id|
| car_id| 是 | int|车辆id|
| car_vin| 是 | string|车辆vin|

     updatetrack array 本次跟进信息
                  
                 track_aim:0,     跟进目的
                 track_method:0,  跟进方式
                 track_result:14, 跟进结果/默认14
                 new_level:0,     跟进级别
                 track_record:'', 跟进理由

     addowner  array  添加车主信息

                     name:'',                string     车主姓名
                     phone:'',               string     电话号码
                     sex:'',                 int        性别
                     birthday:'',            string     生日
                     certificate_type:0,     int        证件类型
                     certificate_code:'',    string     证件编码
                     iscar:false,            boolean    是否提车

     addvisit  array 回访信息
                 
                     plan_date:'',           string     回访日期
                     type:'日常关系维护',     string     回访类型
                     content:0,              int        回访内容
                     visit_id:0,             int        被回访人

      addcar   array 车辆信息
                     sell_date:'',           string     销售日期
                     buy_money:0,            float      购买价格
                     pay_method:0,           int        购买方式
                     boutique_money:0,       float      精品销售总额

     return  0 添加失败      1 添加成功 