### **请求接口**
index.php?app=Car&m=VisitMobile&a=editVisit



### **公网测试**
http://www.apps.com/index.php?app=Car&m=VisitMobile&a=editVisit

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| updatevivit| 是 | array|本次回访信息|
| id| 是 | int|跟进表id|
| client_id| 是 | int|客户id|
| addvisit| 是 | array|下次回访信息|

     updatevisit array 本次回访信息
                  
                 visit_id:0,     被回访人
                 visit_name:'',  被回访人姓名
                 content:0,      回访内容
                 plan:0,         回访计划
                 satisfied:0,    满意度
                 record:'',      回访记录

     addvivit  array  下次回访信息

                 plan_date:'',       计划回访时间
                 type:'日常关系维护', 类型
                 content:0,          回访内容
                 visit_id:0,         被回访人

     return  0 添加失败      1 添加成功