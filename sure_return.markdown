### **请求接口**
/index.php?app=Asset&m=AsserApi&a=sure_return



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=sure_return

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| id     | 是 |   审核表的id   |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status         |1.更新成功；0. 更新失败 |int    |操作状态编号  |
|info     | -------     |1.更新成功；0. 更新失败   |操作状态信息    |


### **示例**
````php
{
status: 1,
info: "更新成功"
}