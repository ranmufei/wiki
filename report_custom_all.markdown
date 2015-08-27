## 客户类型
### **请求接口**
/index.php?app=Customer&m=Mreport&a=custom_all

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=Mreport&a=custom_all&access_token=

### **公共参数** 
`暂无`

### **其他参数**
无


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript
[
{
name: "客户线索",
y: 15.43,
count: "52"
},
{
name: "客户(无订单)",
y: 84.57,
count: "285"
},
{
name: "成单客户",
y: 0,
count: "0",
sliced: true,
selected: true
}
]