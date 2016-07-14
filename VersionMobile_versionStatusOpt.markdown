### **需求报价/版本操作/版本状态修改操作**
index.php?app=InquiryManageClothing&m=VersionMobile&a=versionStatusOpt

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=VersionMobile&a=versionStatusOpt&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|   类型  |说明      |
|------|-----|------|------|
| vid| 是 | int|版本vid|
| status| 是 | int|状态|
| reason| 是 | string|操作理由|
| price| 是 | float|重新报价价格(只有当status = 8 是 才必填)|

     status  :  状态  1   : 确定信息提交到技术审核
                         11  : 版本作废操作(最开始版本作废) 
                         5   : 版本定版(重定版)操作
                         6   : 版本待版状态
                         7   : 版本作废
                         8   : 版本重新报价操作

