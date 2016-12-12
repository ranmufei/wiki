### **请求接口**
index.php?app=AfterSalers&m=FxdMobile&a=fxdOrderSh_tg



### **公网测试**
http://www.apps.com/index.php?app=AfterSalers&m=FxdMobile&a=fxdOrderSh_tg&access_token=

### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
|id|是|售后单id|
|sh_reply_text|是|审核意见|
|type|是|1 存在处理方式为技术检测的  2 技术检测审核通过  3 我的线索审核通过但没添加商品的 0 其他|
|ids|是|array 技术检测审核通过才有 cl_method=7的 即处理方式为现场完成，维修单id|
|log_type|是|1 我的线索审核通过  2 技术检测审核通过 3 售后单审核通过 4 审核通过|
|rep_info|是|array 有商品的时候就必须填  包括（id：维修单id  cl_method：处理方式  cl_person：处理人） |
|ok|是|array 维修单id 我的线索审核通过才有 cl_method=8的 即处理方式为已完成|
|id_arr|是|array 处理人id cl_method=6的 即处理方式为技术检测 |
|jc_id|是|我的线索审核通过但没添加商品的 选择的审核人id|

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
