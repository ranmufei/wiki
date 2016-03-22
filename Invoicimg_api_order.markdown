### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=getOrderlist

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getOrderlist

退货
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getOrderList&cg=4&paystatu=1&ordertype=1&p=undefined&cate_id=undefined&str=undefined&perPages=10
搜索
http://www.apps.com/index.php?app=Invoicimg&m=Supply&a=getOrderList&ordertype=0&cg=4&p=0&cate_id=0&str=搜索内容&perPages=10

### **需要的参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|ordertype         |  0            |int|订单类型         |
|cg|              |int|4未审核订单；1是已经审核 2是已入库 3审核未通过|
|perPages       |              |int    | 每页显示的数量 已经给25 |
|p      |              |int    | 当前显示页  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|data      |         | array |返回数组 |
|count      |         | int | 总数 |

``` javascript


statu: 1,
info: "ok",
data: {
count: "334",
totalPages: 34,
nowPage: 1,
html: "<ul><li> <li class='active'><a href='javascript:' >1</a></li><li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=2'>2</a></li><li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=3'>3</a></li><li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=4'>4</a></li><li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=5'>5</a></li> <li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=2'>下一页</a></li> <li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=6' >下5页</a></li> <li><a href='/index.php?m=Supply&a=getOrderList&app=Invoicimg&ordertype=0&cg=1&perPages=10&p=34' >最后一页</a></li> &nbsp;&nbsp;NUM:334 1/34 页</li></ul>",
data: [
{
id: "1482",
uid: "1",
order_num: "CG2016312164846 (<span style="color:green">审核通过</span>)",
gys_id: "",
creat_time: "2016-03-12",
count_price: 30484,
num: "2.00",
orderstatu: "0",
ordertype: "0",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "0",
default6: "0",
line_status: "0",
is_bigorder: "0",
gys_name: null,
adminName: "庆丰包子",
intoStoreNum: "0.00",
stornstatu: 0,
is_open: false,
paystatu: 0
},
{
id: "1477",
uid: "1",
order_num: "CG2016312145729 (<span style="color:green">审核通过</span>)",
gys_id: "0",
creat_time: "2016-03-12",
count_price: 354,
num: "1.00",
orderstatu: "0",
ordertype: "0",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "1",
default6: "0",
line_status: "1",
is_bigorder: "0",
gys_name: null,
adminName: "庆丰包子",
intoStoreNum: "0.00",
stornstatu: 0,
is_open: false,
paystatu: 0
},
{
id: "1434",
uid: "1",
order_num: "CG201634164320 (<span style="color:green">审核通过</span>)",
gys_id: "0",
creat_time: "2016-03-04",
count_price: 12,
num: "1.00",
orderstatu: "0",
ordertype: "0",
to_address: null,
ckid_1: "0",
ckid_2: "0",
is_pd: "0",
type: "1",
default6: "0",
line_status: "0",
is_bigorder: "0",
gys_name: null,
adminName: "庆丰包子",
intoStoreNum: "0.00",
stornstatu: 0,
is_open: false,
paystatu: 0
},