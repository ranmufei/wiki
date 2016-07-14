### **物料操作/物料单耗修改**
index.php?app=InquiryManageClothing&m=TechnologyMobile&a=save_data

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=TechnologyMobile&a=save_data&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
post

(物料的用量不能小于0 , 损耗数只能在0-100)
### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| vid| 是 | int|版本 vid|
| id| 是 | int|物料id|
| val| 是 | float|当前修改的值|
| type| 是 | int|修改类型( 1: 数量 , 2 : 价格 , 3:损耗 )|
| k_price| 是 | float|单个物料的总价|
| total_price| 是 | float|总成本|
| m_price| 是 | float|总的物料成本|
| wastage_price| 是 | float|总的损耗成本|
|profit| 是 | float|总的利润|
| is_other_price| 是 | int|0 (固定死)|
