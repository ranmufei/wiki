### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=getOutStronProductPici

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getOutStronProductPici&access_token=e133ac84d35628422ca6c2c408667a&formatid=1051&ckid=32

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|formatid|              |string |产品规格id  |
|ckid|              |string |仓库id  |
|p|              |string |分页  |
|str|              |string |搜索内容  |
### **其他参数**
无

### **显示字段** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|intobatch|              |string |批次号  |
|stornhouse|              |string |仓库名称  |
|time|              |string |入库时间|
|stronNum|              |string |库存剩余量  |

``` javascript
{
count: "2",
totalPages: 1,
nowPage: 1,
data: [
{
id: "356",// 批次id
orderid: "2881",
proid: "382", 
subid: "1051",
adminUid: "1",
time: "2016-06-21 15:52",
stornhouseid: "32",
type: "6",
mark: null,
pici: "2",
default2: null,
productdate: "1466438400",
intobatch: "yds_ksd_HJJK", //批次号
num: "50", 
stronNum: "50", //批次剩余库存数量
statu: "0",
isdelete: "0",
surplus: "50",
format: "fa_-9999-9999_0", 
xlh_length: "0",
stornhouse: "是是是是", //仓库名称
productiontimes: "2016-06-21 00:00",
batchcode: "1466495456831",
disable: false,
justday: "【已入库1天】",
bzq: false
},
{
id: "354",
orderid: "2881",
proid: "382",
subid: "1051",
adminUid: "1",
time: "2016-06-21 15:50",
stornhouseid: "32",
type: "6",
mark: null,
pici: "1",
default2: null,
productdate: "1466438400",
intobatch: "ys_AD_ds",
num: "50",
stronNum: "50",
statu: "0",
isdelete: "0",
surplus: "50",
format: "fa_-9999-9999_0",
xlh_length: "50",
stornhouse: "是是是是",
productiontimes: "2016-06-21 00:00",
batchcode: "1466495456831",
disable: false,
justday: "【已入库1天】",
bzq: false
}
]
}