### **请求接口**
index.php?app=Car&m=ManageRecordMobile&a=status



### **公网测试**
http://www.apps.com/index.php?app=Car&m=ManageRecordMobile&a=status

### **请求方式**
get


### **参数**
无    

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|data|-------   |array  |状态列表  |

      data：array  状态列表
            
           data['deal_status']  处理状态  array
                  id             int
                  deal_status    string
