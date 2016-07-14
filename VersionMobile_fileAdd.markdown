### **需求报价/版本操作/新增附件**
index.php?app=InquiryManageClothing&m=VersionMobile&a=fileAdd

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=VersionMobile&a=fileAdd&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| vid| 是 | int|版本vid|
| data| 是 | array|附件数据|
data :  array 附件数据 
                      [0][id]          // 索引id
                      [0][name]        // 附件名
                      [0][file]        // 附件地址
                      [0][show_file]   // 附件显示地址
                      [0][type]        // 附件类型
                      [0][downurl]     // 下载id