### **请求接口**
/index.php?app=Asset&m=AsserApi&a=consumable_list



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AsserApi&a=consumable_list



### **返回结果**
|字段        |值             |类型    |说明        |
| ---------  |--------       |--------|--------    |
|id          |-------  |int  |物品id   |
|number| ------         |array   |物品编号  |
|type| ------         |array   |目前未用  |
|already_num| ------         |array   |申租品已经借出数量  |
|ntime|   -----       |     |  购买时间   |
|names      |------      |-----   |物品名称      |
|old|    |　　　｜　折旧率　｜
|is_old|    |　　　｜　是否属于折旧　｜
|num|       |       |    string     | 物品数量|
|remark|       |       |    string     |  备注信息|
|gunit|       |       |    string     | 物品单位|
|cateid|       |       |    string     |  大分类（1）易耗品（2）申租品（3）折旧品|
|buytime|       |       |    string     |  添加时间|
|price|       |       |    string     |  物品单价|
|now_tprice|    |  | 数量*单价后 折旧的价格 |
|img|       |       |    string     |  物品图片地址|
