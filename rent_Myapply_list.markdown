### **请求接口**
/index.php?app=Asset&m=AsserApi&a=rent_Myapply_list



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=rent_Myapply_list

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   当前登录用户id   |


### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|id          |-------   |int    |物品id   |
|number      | -------     |varchar  |物品编号      |
|names       |-------     |varchar   |物品名称      |
|applytime| -------     |   varchar        |  申请时间     |
|cat| -------    |varchar  |分类     |
|state| -------     |int  |审核状态     |
|reject| -------     |int  |驳回信息     |


### **示例**
````php
{
id: "143",
img: "./Uploads/2015/0502/18/5544a19a129a2.jpg",
number: "shenzhu_00211",
names: "电脑",
applytime: "1434511491",
cat: "9",
num: "3",
state: "待审批"
},