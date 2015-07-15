## 订单 支付记录
### **请求接口**
/index.php?app=Customer&m=MMidOrder&a=pay_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MMidOrder&a=pay_info&id=43&access_token=

### **公共参数** 

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |机会id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | {} ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
amount: "4444.00",      //总金额
pay: "289.00",          //已交易
remain: "4155.00",      //剩下
opt: "0",               //0收款 1支出 (暂时不需要显示)
logs: [                 //支付记录列表
{
amount: "256.00",                //金额
inputtime: "2015-07-15 11:42",   //创建时间
userid: "1",                     //创建人ID
username: "庆丰包子"             //创建人改名
},
{
amount: "33.00",              
inputtime: "2015-07-03 11:03",
userid: "1",
username: "庆丰包子"
}
]
}