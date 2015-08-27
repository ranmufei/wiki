## 销售机会阶段
### **请求接口**
/index.php?app=Customer&m=Mreport&a=chance_stage

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=Mreport&a=chance_stage&access_token=

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
[
"初步接洽",
13
],
[
"需求确定",
11
],
[
"方案/报价",
7
],
[
"谈判审核",
5
],
[
"赢单",
5
],
[
"输单",
1
]
]