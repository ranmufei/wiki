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
|dimension|              |string |扫描二维码或者条码返回的信息  |
|ckid|              |string |选中仓库时必须带仓库id  |
### **其他参数**
无



``` javascript
{
info: [
{
id: "4554",
order_id: "2874", //订单id
pro_id: "382", //产品id
xinhao: "1051", // 规格id
unit: "335",
price: "60.00", //单价
num: "2.00",  //出入库的数量
intoStoreNum: "0.00", // 已近出入库的数量
stornNum: 0, // 对应仓库的库存数量
ckid: "2" // 出库的仓库id
},
{
id: "4555",
order_id: "2874",
pro_id: "382",
xinhao: "1052",
unit: "335",
price: "30.00",
num: "3.00",
intoStoreNum: "0.00",
stornNum: 0,
ckid: "2"
}
]
}