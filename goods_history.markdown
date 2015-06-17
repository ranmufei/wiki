### **请求接口**
/index.php?app=Asset&m=AsserApi&a=goods_history



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=goods_history

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   物品id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|userid| -------     |varchar  |申请人姓名    |
|applyuid|-------     |varchar   |批注人姓名|
|applytime| -------     |   varchar        |  申请时间     |
|goodsid| -------    |varchar  |物品id|
|applytime| -------     |int  |申请时间    |
|num| -------     |int  |申请数量    |
|is_delete| -------     |int  |是否删除 ‘1’：未删除， ‘0’：已删除   |


### **示例**
````php
{
id: "96",
userid: "庆丰包子",
applyuid: "庆丰包子",
goodsid: "183",
cateid: "1",
borrowtime: "",
reurntime: "",
applytime: "2015-06-16 09:06",
state: "",
num: "2",
is_delete: "1",
one: "",
two: "",
three: ""
},