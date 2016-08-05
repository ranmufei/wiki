### **请求接口**
index.php?app=Car&m=OwnerMobile&a=getbackCar



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OwnerMobile&a=getbackCar

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   车主id  |
| client_id| 是 |   1 客户id  |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status| -------     |array    |退换车类型     |
|owner| -------     |array    |车主信息    |
|car| -------     |array   |车辆信息     |

{
   status: [
       {
           id: "6",
           status: "换车申请"
       },
       {
            id: "7",
            status: "退车申请"
       }
   ],
   owner: {
        id: "21",
        client_id: "75",
        name: "废物",
        phone: "13349888266",
        certificate_type: "身份证",
        certificate_code: "wqer32 "
   },
   car: {
        menu: {
        param0: "颜色",
        param1: "内存"
   },
   product: [
        {
        car_vin: "qw ",
        id: "23",
        name: "苹果",
        format: "iphone6s",
        price: "6000.00",
        specs: [
                  {
                      value: "白色"
                  },
                  {
                      value: "16G"
                   }
               ]
         }
    ]
  }
}