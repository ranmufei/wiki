### **请求接口**
/index.php?app=Asset&m=AssetApi&a=rent_cat



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=rent_cat



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |分类id   |
|pid      | -------     |int  |分类的父级id      |
|name| -------    |varchar  |分类的名称      |

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