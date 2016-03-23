### **请求接口**
/index.php?app=Invoicimg&m=SaleMobile&a=mysalebills

### **接口说明**
`分页`

### **请求方式**
get/post

### **浏览器查看（我的对账单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mysalebills&p=1&access_token=

### **浏览器查看（对账单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=salebills&p=1&access_token=

### **浏览器查看（我的对账单详情列表）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mygysbill&p=1&access_token=

### **浏览器查看（对账单详情列表）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=gysbill&p=1&access_token=

### **公共参数** 
`num`、`p`

### **其他参数**
str        搜索客户（我的对账单、对账单）
timestart  筛选的开始时间（我的对账单、对账单）
timeend    筛选的结束时间 （我的对账单、对账单）
userid     筛选的员工 （对账单）


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------|--------|--------       |
|statu| |||
|data |array  |array  | 如下 |
|info| '' | |   |

``` javascript
//没有数据 的情况（info: "error"、statu: 0   ）
[
{    
data: null 
}
]

//有数据的情况（我的对账单、对账单）
[
{
count: "11",
nopay: 2710213.6   //未付
pay: 1068.2        //已付
sum: 2711281.8     //总金额
data: [
{
count: 1           //订单数量
gys_id: "303"                        
gys_name: "目录可以解读"  //客户
money: 48000         //订单应收
nopay: 48000   //待收金额
num: 8        //销售数量
pay: 0        //已收金额
}
.....
]
}
]