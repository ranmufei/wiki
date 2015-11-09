### **请求接口**
/index.php?app=Cws&m=MApi&a=cashflowReport

### **接口说明**

### **请求方式**
post

### **浏览器查看**
http://www.apps.com/index.php?app=Cws&m=MApi&a=cashflowReport

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
|data       |array         |array  | cname : 客户名称; contact：联系人;  state:状态; createtime:创建时间; post:职务 ; id:ID |
|info       | '' | string | 接口状态说明  |

