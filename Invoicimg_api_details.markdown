### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=getProductInfo


### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getProductInfo

### **参数**
id // 产品id





## 返回结果
##产品详情
|info|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|id| |int|产品id|
|brand||string|品牌|
|code||string|编码|
|time||varchar|创建时间|
|countNum||varchar|库存总数|
|cate_name||varchar|分类名|
|custom_name||varchar|供应商|
|dw||varchar|单位|

## 规格库存
|proList|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|id| |int|规格id|
|purchasePrice||string|采购价|
|stornPrice||string|库存成本|
|sellPrice||varchar|销售价|
|barcode||varchar|条码|
|stornNum||varchar|库存数量|
|param0||varchar|规格一|（有则显示）
|param1||varchar|规格二|（有则显示）



## 销售记录
|SaleProice|string| | 最小-最大 |

## 采购记录
|PurchaseProice|string| | 最小-最大 |


##产品详情
|storn|array | 类型 | 返回数据 数组|
|----|----|----|-----|
|stornName| |varchar|仓库名|
|storn|array | | 产品规格数组|
|param0| |varchar|产品规格一|(有则显示)
|param1| |varchar|产品规格二|(有则显示)
|formatNum| |varchar|库存数量|
|formaname| |varchar|规格名|


