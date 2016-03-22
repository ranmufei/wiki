### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=get_intoutInfo

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=get_intoutInfo&ckid=1&access_token=e133ac84d35628422ca6c2c408667a

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|ckid       |              |string |仓库id|
|start       |              |string |查询开始时间|
|end       |              |string |结束时间|
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data|         | array|数组 |
|count|         | string |总条数|
