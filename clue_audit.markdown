### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=Sh_tg



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=Sh_tg&access_token=

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
|id|是|售后单id|
|sh_reply_text|是|审核意见|
|type|是|1 我的线索审核通过  2 技术检测审核通过  3 售后管理审核通过|
|jc_id|是|我的线索审核通过但没添加商品的 选择的审核人id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
status 1 成功 其他失败
info   失败原因