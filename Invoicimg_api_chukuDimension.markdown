### **请求接口**
/index.php?app=Invoicimg&m=InstockApi&a=getStrorageList

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=getStrorageList&access_token=e133ac84d35628422ca6c2c408667a

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|dimension|              |string |扫描二维码或者条码返回的信息  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|orderinfo|         | object|订单基本信息 |
|list|         | array| 产品信息|
|wuliudetail|         | array | 物流订单信息 |
|wuliudetail[0][wl_dynamic]|         | array | 物流动态|
|piciInfo|         | array | 批次记录 |
|xulieInfo|       | array | 序列号记录 |

``` javascript