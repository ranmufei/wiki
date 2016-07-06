### **获取所有版本列表**
index.php?app=InquiryManageClothing&m=TechnologyMobile&a=getDataLists

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=TechnologyMobile&a=getDataLists&access_token=67f244a585df480f51e9b81037f6d4&pageSize=10&p=1

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| pageSize| 是 |   每页分页条数|
| p     | 是 |   当前页   |
| type| 是 |   版本状态 (1:全部 , 2:未操作 , 3: 已操作)  |
| enter_type| 是 |   'index' (必须带,固定死) |
| model_name     | 是 |   index'(技术核价) , 'need'(需求核价) , 'sure'(报价审核) |

