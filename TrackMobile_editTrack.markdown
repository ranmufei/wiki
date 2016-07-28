### **请求接口**
index.php?app=Car&m=TrackMobile&a=editTrack



### **公网测试**
http://www.apps.com/index.php?app=Car&m=TrackMobile&a=editTrack

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| updatetrack| 是 | int|本次跟进信息|
| id| 是 | int|跟进表id|
| client_id| 是 | int|客户id|
| client_level| 是 | int|客户级别|
| orginal_status| 是 | int|客户状态|
| addtrack| 是 | array|下次跟进信息|
| orderid| 是 | int|订单id|

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
     return  0 添加失败      1 添加成功