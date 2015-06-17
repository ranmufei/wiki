### **请求接口**
/index.php?app=Asset&m=AsserApi&a=number_not_rent



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=number_not_rent

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   申租品的id  |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |编号id   |
|number      | -------     |varchar  |物品编号      |
|goodsid |-------     |varchar   |对应的物品id      |
|state|-------     |varchar   |出租状态      |
|is_delete|-------     |varchar   |是否删除状态 1.未删除2.已删除     |
|goodsid |-------     |varchar   |对应的物品id      |




### **示例**

````php
{
id: "63",
number: "ls_918681340012",
goodsid: "91",
cat: null,
state: "未出租",
uid: null,
is_delete: "1",
one: null,
two: null,
three: null
},