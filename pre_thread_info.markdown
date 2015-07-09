## 获取线索详情
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=view_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrethread&a=view_info&id=331

### **公共参数** 

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |线索id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
id: "331",
charge: "庆丰包子",
cname: "武汉科技大学",
contact: "江丽",
state: "已联系",
sex: "男",
depart: "信息化研究部",
post: "经理",
phone: "3131313131",
mobile: "1313131313",
email: "",
weibo: "",
area: "",
address: "",
code: "",
source: "",
remark: "",
userid: "庆丰包子",
createtime: "06-26 11:26",
change: "0"
}