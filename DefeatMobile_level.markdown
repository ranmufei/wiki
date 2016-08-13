### **请求接口**
index.php?app=Car&m=DefeatMobile&a=process



### **公网测试**
http://www.apps.com/index.php?app=Car&m=DefeatMobile&a=process&access_token= 

### **请求方式**
post


### **参数**
|参数        |必填          |类型    |说明        |
| ---------  |--------    |-------- |--------  |   
|process_opinion|是  |string  |处理意见  |
|id|是  |int  |战败id  |
|deal_status|是 |int  |处理结果  1 同意  2 驳回  3 分配其他  |
|nsale_id|是  |int  |销售顾问id  |

### **返回结果**
  0 失败  1 成功