### **请求接口**
index.php?app=Car&m=ManageRecordMobile&a=getSelect



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageRecordMobile&a=getSelect

### **请求方式**
post

### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| perPages| 是 | int|每页显示条数，默认10|
| getSelect| 是 | array|本次跟进信息|

     getSelect  array 筛选数据
            deal_status   int  处理状态
            

     return  0 添加失败      1 添加成功