### **请求接口**
index.php?app=AfterSalers&m=FxdclZxMobile&a=createSupOrder


### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdclZxMobile&a=createSupOrder&access_token=

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| data| 是 |array 具体如下|
Supdata:{   //物料单对应的数据
            rid:'',   //售后单id
            r_order:'',  //售后单 order
            c_id:'',     //顾客id
            c_name:'',  //顾客name
            sh_uid:'',  //审核人 id
            js_id:'',    //经手人 id
            js_uname:'',   //经手人name
            remark:'',   //备注
            supplies:[],  //物料
            num:0,        //物料数量
        },