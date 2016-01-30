### **我的客户列表**

### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrecustom&a=lists&sta=1&access_token=
### **公共参数** 
`num`、`p`

### **其他参数**
sta 默认不传（1为我参与的，2为我下属的）

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | count:总数据量 , totalPages:总页数 ， nowPage:当前页 , data:[]数据列表(具体查看以下代码) |
|info       | '' | string | 接口状态说明  |

``` javascript
data: [
{
custom_company: "武汉大学",    //客户名称
level :''                     //重要级别
custom_type: "代理商",        //客户类型
sales: "",                   //年销售额
inputtime ：'2015-07-03 14:56' //创建时间
id: "277"                    //客户ID
is_leave: "0"                //是否离职  ，1为离职（庆丰包子（离职））,0为（庆丰包子）   
apportion_id: "庆丰包子"      //负责人
},
]