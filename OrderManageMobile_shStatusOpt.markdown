### **订单管理/订单审核操作**
index.php?app=InquiryManageClothing&m=OrderManageMobile&a=shStatusOpt

### **公网测试**
http://www.apps.com/index.php?app=InquiryManageClothing&m=OrderManageMobile&a=shStatusOpt&access_token=67f244a585df480f51e9b81037f6d4

### **请求方式**
get


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| id| 是 |   订单id|
| sh_comments| 是 |   审核评语(必须)|
| sh_status| 是 |   审核状态 (
                            1 :  通过并提交给一个人审核 (转审必须要传sh_uid)
                            2 :  审核通过
                            3 :  驳回操作,订单作废
                        )|
| sh_uid| 是 |  转审审核人uid (如果没有填 0 )(必须)|
