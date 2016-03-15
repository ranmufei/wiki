### **请求接口**
/index.php?app=Invoicimg&m=ProductApi&a=avalon_cg_info

### **接口说明**
`订单详细信息`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=avalon_cg_info

### **需要的参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|type|  0/1            |int|0收款 1是付款         |
|id      |              |int    | 订单的id  |
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |

``` javascript

list: [
{
id: "2154",
order_id: "1471",
pro_id: "148",
ctime: "1457681697",
uid: "6",
cid: "0",
name: "",
b_no: null,
xinhao: "370",
unit: "92",
price: "354.00",
num: "1.00",
intoStoreNum: "0.00",
count_price: "0.00",
discount: "100",
isdelete: "0",
supplier_id: "26",
g_time: "1457798400",
title: null,
price_time: "1970-01-01",
address: null,
already_num: "0",
default1: "0",
default2: "0",
unitname: "双",
unitinfo: {
id: "92",
pid: "148",
unitid: "52",
relation: "1",
default: "1",
delete: "0",
default1: "0",
default2: "0",
default3: "0",
default4: "0"
},
unitnum: 1,
proName: "球鞋",
formatname: "QX_BS-DH_2",
intonum: "1.00",
supplier_name: [
"正正的测试"
],
supplier_count: 1,
param0: "白色",
param1: "大号"
}
],
tableHeader: {
param0: "颜色",
param1: "大小"
},
sns: null,
log: [ ],
goods_address: false
}