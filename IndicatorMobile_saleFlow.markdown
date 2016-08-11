### **请求接口**
index.php?app=Car&m=IndicatorMobile&a=addClient



### **公网测试**
http://www.apps.com/index.php?app=Car&m=IndicatorMobile&a=addClient&date=2016-7-22&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| date| 是 | string|日期| 

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|data|-------   |array  |建卡量统计  |

      data：array  建卡量统计
            
            sale_id    销售顾问id
            sale_name  销售顾问姓名
            recep      接待建卡数量
            phone      开拓建卡数量
            count      合计
