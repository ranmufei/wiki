### **物料操作/物料删除**
index.php?app=InquiryManageClothing&m=TechnologyMobile&a=delVersionMaterial

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=TechnologyMobile&a=delVersionMaterial&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
post


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| vid| 是 | int|版本vid|
| ids| 是 | array|删除的物料id|
| sid| 是 | int|规格sid|
| price| 是 | int|版本价格列表|

   price : array 版本价格表
                price[material_price]     // 物料总成本
                price[wastage_price]      // 损耗总成本
                price[other_price]        // 其他价格
                price[profit]             // 利润
                price[total_price]        // 总价