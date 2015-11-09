### **请求接口**
/index.php?app=Cws&m=MApi&a=getCashflowReport

### **接口说明**

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Cws&m=MApi&a=getCashflowReport

### **公共参数** 

### **其他参数**
### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|timetype   |时间段类型  本周: thisweek(默认值)、本月：thismonth、上月：lastmonth、今年：thisyear、去年：lastyear、custom：自定义时间段 |    string|
|start     |开始时间（timetype=custom时生效） | string |          |
|end     |开始时间（timetype=custom时生效） | string |          |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  |请看下面代码 |
|info       | '' | string | 接口状态说明  |


``` javascript
data: {
collect: {          //收入
sum: "1233.00",
info: [             //收入名细
{
name: "客户管理订单",
count: 0,
percent: "0.00"
},
{
name: "进销存收款",
count: 0,
percent: "0.00"
},
{
name: "销售订单收款",
count: "1233.00",
percent: "100.00"
},
{
name: "样品出借",
count: 0,
percent: "0.00"
},
{
name: "连锁收银收款",
count: 0,
percent: "0.00"
}
],
percent: "100.00"
},
pay: {        //支出
sum: "0.00",
info: [      //支出名细
{
name: "固定资产采购",
count: 0,
percent: "0.00"
},
{
name: "固定资产维修",
count: 0,
percent: "0.00"
},
{
name: "进销存付款",
count: 0,
percent: "0.00"
},
{
name: "销售订单付款",
count: 0,
percent: "0.00"
},
{
name: "连锁收银付款",
count: 0,
percent: "0.00"
},
{
name: "在线报销",
count: 0,
percent: "0.00"
}
],
percent: "0.00"
},
margin: "1233.00"
},
