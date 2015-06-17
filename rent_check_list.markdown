### **请求接口**
/index.php?app=Asset&m=AsserApi&a=rent_check_list



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=rent_check_list



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|number      | -------     |varchar  |物品编号      |
|names      | -------     |varchar  |物品名称      |
|userid| -------    |varchar  |申请人id     |
|applytime| -------     |int  |申请时间     |
|cat|  -------   |varchar     |  分类   |
|num|-------     |varchar   |申请数量      |
|img|  -------         |   varchar  |  物品图片地址    |
|state|   -------         |varchar　　|　申请状态 |
|remark| -------   |int　|　申请备注     |
### **示例**
````php
{
id: "143",
number: "shenzhu_00211",
names: "电脑",
img: "./Uploads/2015/0502/18/5544a19a129a2.jpg",
userid: "1",
applytime: "1434511491",
cat: "9",
num: "3",
state: "待审批",
remark: "",
goodsid: "59"
},