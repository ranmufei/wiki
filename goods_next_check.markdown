### **请求接口**
/index.php?app=Asset&m=AsserApi&a=goods_next_check



### **公网测试**
http://www.apps.com//index.php?app=Asset&m=AssetApi&a=goods_next_check

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| apply_id| 是 |   本条信息的id  |
| word| 是 |   备注内容  |
| status| 是 | 提交审批人的id    |
| uid| 是 |   操作人uid  |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|statu         |1.提交成功；0. 提交失败  3. 提交人不能是自己 4. 该审核人没有权限 |int    |返回状态  |
|info     | -------     |   |操作状态信息    |

