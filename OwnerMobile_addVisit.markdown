### **请求接口**
index.php?app=Car&m=OwnerMobile&a=addVisit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=OwnerMobile&a=addVisit

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| isputcar| 是 | int|0 提车  1 延迟提车|
| id| 是 | int|车主id|
| client_id| 是 | int|客户id|
| addvisit| 是 | array|下次回访信息|

     addvisit  array  下次回访信息

                 plan_date:'',       计划回访时间
                 type:'日常关系维护', 类型
                 content:0,          回访内容
                 visit_id:0,         被回访人

     return  0 添加失败      1 添加成功