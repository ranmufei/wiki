### **请求接口**
/index.php?app=Asset&m=AsserApi&a=consumable_list



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AsserApi&a=consumable_list



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|number      | -------     |varchar  |物品编号      |
|type        | -------    |varchar  |目前未用      |
|already_num | -------     |int  |申租品已经借出数量     |
|ntime       |  -------   |varchar     |  购买时间   |
|names       |-------     |varchar   |物品名称          |
|old         |   -------         |varchar　　|　折旧率 |
|is_old| -------   |int　|　是否属于折旧     |
|num |    -------         |int | 物品数量 |
|remark|  -------      | varchar   |  备注信息   |
|gunit|   -------        |  varchar | 物品单位|
|cateid|   -------       |  int  |  大分类（1）易耗品（2）申租品（3）折旧品|
|buytime|  -------        | varchar    |  添加时间   |
|price|   -------          |   float |  物品单价    |
|now_tprice        | -------     | varchar   | 数量*单价后 折旧的价格   |
|img|  -------         |   varchar  |  物品图片地址    |