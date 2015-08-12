### **请求接口**
/index.php?app=Eboss&m=EbossApi&a=getsell_day



### **公网测试**
http://www.apps.com/index.php?app=Eboss&m=EbossApi&a=getsell_day

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|ordernum|-------   |int    |出勤今日销售订单|
|orderprice| -------     |int    |今日销售总额     |
|sale|-------   |int    |今日毛利润  |
|daycaigouCount| -------     |int    |今日采购订单     |
|daycaigouCountPrice|-------   |int    |今日采购总金额 |

### **示例**
````php
{
ordernum: "0",
orderprice: 0,
sale: 0,
daycaigouCount: "0",
daycaigouCountPrice: 0
}