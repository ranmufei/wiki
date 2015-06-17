### **请求接口**
/index.php?app=Asset&m=AsserApi&a=consumable_Myapply_list



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=consumable_Myapply_list

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


### **示例**
````php
data: [
{
id: "142",
img: "",
number: "yh_20150612104561",
names: "软件易耗品上传测试2",
applytime: "1434419208",
cat: "14",
num: "2",
state: "审核通过"
},
