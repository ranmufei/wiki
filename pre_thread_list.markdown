### **请求接口**
/index.php?app=Customer&m=MPrethread&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrethread&a=lists

### **公共参数** 
`num`、`p`

### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | cname : 客户名称; contact：联系人;  state:状态; createtime:创建时间; post:职务 ; id:ID |
|info       | '' | string | 接口状态说明  |

``` javascript
[
{
cname: "saDSA",
contact: "ASDASd",
mobile: "122345662144",
phone: "1232131231",
post: "",
state: "",
createtime: "11-12 17:16",
id: "453"
},
……
]