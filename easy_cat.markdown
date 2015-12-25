### **请求接口**
/index.php?app=Asset&m=AssetApi&a=easy_cat



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=easy_cat



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|number      | -------     |varchar  |物品编号      |
|type        | -------    |varchar  |目前未用      |
|already_num | -------     |int  |申租品已经借出数量     |
### **示例**
````php
[
{
id: "8",
pid: "0",
name: "1111"
},
{
id: "12",
pid: "0",
name: "劳保"
},
{
id: "104",
pid: "0",
name: "生活用品"
},
{
id: "115",
pid: "0",
name: "11",
children: [
{
id: "118",
pid: "115",
name: "444"
}
]
}
]