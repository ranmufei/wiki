## **获取所有客户**
`可根据 姓名/首字母/全拼 作模糊查询`

### **请求接口**
/index.php?app=Customer&m=MIndex&a=custom_list

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MIndex&a=custom_list

### **公共参数** 
`num`、`p`

### **其他参数**
无

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |

``` javascript
 {
count: "1",
totalPages: 1,
nowPage: 1,
data: [
{
custom_company: "客户名称",
level: "A(重点客户)",
custom_type: "扣子供应商",
sales: "",
inputtime: "2015-12-08 14:42",
id: "369"
}
]
}