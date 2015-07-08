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
|data       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|uid        |              |String |员工id  |
|name       |              |string |员工姓名   |
|postName   |              |String |员工职位名  |
|spelling   |              |String |员工姓名拼音全拼(小写) |
|abbreviation |            |String |员工姓名拼音首字母(大写) |
|change	(暂时未加入) |      |boolean|true有修改 ，false没有修改 |

