## 订单每月
### **请求接口**
/index.php?app=Customer&m=Mreport&a=order_data

### **接口说明**

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=Mreport&a=order_data&access_token=

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
{
x: [
"2015-01",
"2015-02",
"2015-03",
"2015-04",
"2015-05",
"2015-06",
"2015-07",
"2015-08"
],
data: [
0,
0,
0,
9,
11,
20,
3,
0
]
}