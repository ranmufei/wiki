### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=get_Batch_list

### **接口说明**
`分页`

### **请求方式**
post,get都可以

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p       | 默认值   |string |分页|


### **浏览器查看**
按批次查看  http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=get_Batch_list&access_token=e133ac84d35628422ca6c2c408667a






### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|p       | 默认值   |string |分页|
|date    | 非必填   |string |保质期检索时的参数 |
|type    | 默认值   |string |1 全部产品 ，2过期产品  ，3 保质期预警  |
按商品查看 http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=InstockApi&a=getBatchList&p=1&type=1&date=2016-07-21&access_token=3fa43a3f8eafd2df4cd10ea6d6e749

