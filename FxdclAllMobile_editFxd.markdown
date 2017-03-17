### **请求接口**
index.php?app=AfterSalers&m=FxdclAllMobile&a=editFxd



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdclAllMobile&a=editFxd&access_token=

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 | 维修单id |
info[money]:0           //金额

info[period_type]:11    //报修类型 

info[cl_method]:1       //处理方式

info[zx_person]:1       //处理人--------只在处理方式为自修即cl_method=1时需要

info[yanbao]:1          //延保类型  --------只在处理方式为延保即g_type=5时需要     

info[js_method]:1       //送修方式

info[g_type]:0          //类型   

que:19

### **返回结果**
1成功 0失败