### **查询我的客户列表**

### **说明**
一般为其他接口服务，如要新增客户,须要选择父级客户。或新增联系人,须要选择客户

### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=list_like

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
无

### **公共参数** 
`num`、`p`

### **其他参数**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|value      |'' |string |可以理解为 客户名称包含的字符串         |
|pid        |true|boolean | 如果是存在参数则表示只显示父级客户 |

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
},
]