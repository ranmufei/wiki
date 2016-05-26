### **请求接口**
/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=get_Supplies_Info

### **接口说明**
`分页`

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg_Suppliers&m=ProductApi&a=get_Supplies_Info&access_token=dda0439fd69c3ad9316f6c2f2a0c36

### **公共参数** 
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|id       |              |int |供应商id|
### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info|         | array |返回详情数组 |
|contact|         | int | 联系人数组 |

``` javascript
{
info: {
sup_company: "供应商",
sup_phone: "13545698745",
url: "www.baidu.com",
facsimile: "024764658",
email: ".2464657@qq.com",
mark: "哦啊是假的",
address: "武汉",
creat_time: "2016-02-20 10:57",
uid: "1",
username: "庆丰包子"
},
contact: [
{
id: "1",
sup_id: "供应商",
receiver: "张三",
area: "220802",
address: "中山路大东门七号",
mobile: "13545698745",
phone: "0246587487",
email: "www.asdasd.com",
remarks: "按时",
sort: "0",
check: "1",
uid: "庆丰包子",
creatime: "2016-02-21 11:59",
default: "0",
areas: "吉林省/白城市/洮北区"
},
{
id: "2",
sup_id: "供应商",
receiver: "李斯",
area: "120116",
address: "莱卡金顿啊",
mobile: "13545698745",
phone: "0216564",
email: "213543546@qq.com",
remarks: "asd ",
sort: "1",
check: "0",
uid: "庆丰包子",
creatime: "2016-02-21 12:00",
default: "0",
areas: "天津/天津市/滨海新区"
}
]
}