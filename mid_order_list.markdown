## 我的订单列表
### **请求接口**
/index.php?app=Customer&m=MMidOrder&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MMidOrder&a=lists&id=43&access_token=

### **公共参数** 
`p` `num`

### **其他参数**
无


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
count: "37",
totalPages: 2,
nowPage: 1,
data: [
{
custom_id: "dsfadfewredd",   //客户名称
state: "已确认",             //状态
money: "4444.00",            //金额
inputtime: "2015-07-03 11:02", //创建时间
id: "43"                     //ID
}
]
}