### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrecustom&a=lists&access_token=
### **公共参数** 
`num`、`p`

### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | count:总数据量 , totalPages:总页数 ， nowPage:当前页 , data:[]数据列表(具体查看以下代码) |
|info       | '' | string | 接口状态说明  |

 javascript
data: [
{
custom_company: "武汉大学",
level: "",
custom_type: "代理商",
sales: "",
id: "277"
},
{
custom_company: "qwq",
level: "",
custom_type: "代理商",
sales: "",
id: "276"
},
{
custom_company: "王琪",
level: "",
custom_type: "采购商",
sales: "",
id: "275"
},
