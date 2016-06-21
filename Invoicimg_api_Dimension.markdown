### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=getOrderInfoByDimension

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getOrderInfoByDimension&access_token=e133ac84d35628422ca6c2c408667a&dimension=Sale_XS201662195242-1

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id|              |string | 出库订单id  |
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