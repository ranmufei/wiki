### **订单管理/获取所有订单列表**
index.php?app=InquiryManageClothing&m=OrderManageMobile&a=getDatasList

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=OrderManageMobile&a=getDatasList&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| pageSize| 是 |   每页分页条数|
| p     | 是 |   当前页   |
| _type     | 是 |   订单状态 (0: 待审核 , 1:审核中 , 2:审核通过 , 3: 全部订单 , 4: 已作废订单)|
| enter_type| 是 |   'index' (必须带,固定死)|