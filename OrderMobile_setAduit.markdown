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

     updateclient array 客户信息
                  
                certificate_type:0,    证件类型
                certificate_code:'',   证件编号

     updateorder array  订单信息

                 order_contacts:'',  订单联系人
                 car_contacts:12,    预计提车时间
                 contacts:'',        提车联系人
                 earnest_money:0,    订金

     addaduit array 审核信息
                 
                 apply_explain             审核说明

     return  0 添加失败      1 添加成功      2 车型匹配失败