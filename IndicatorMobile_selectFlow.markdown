### **请求接口**
index.php?app=Car&m=IndicatorMobile&a=selectFlow



### **公网测试**
http://www.apps.com/index.php?app=Car&m=IndicatorMobile&a=selectFlow&year=2016&month=4&access_token=

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| date| 是 | string|年月|  

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|data|-------   |array  |客流量列表  |

      data：array  客流量列表
            
            day    日期
            num    到店人数
            phone  来电人数
