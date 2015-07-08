## 获取线索动态列表
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=view_dynamics

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrethread&a=view_dynamics&id=

### **公共参数** 
`p` `num`

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |线索id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |data: [
{
day: "今天",
info: [
{
id: "66",
title: "",
remark: "我们新",
origin: "0",
location: "",
area: "",
userid: "庆丰包子",
createtime: "10:58"
}
]
},
{
day: "前天",
info: [
{
id: "60",
title: "",
remark: "56251",
origin: "0",
location: "",
area: "",
userid: "庆丰包子",
createtime: "15:19"
}
]
}
]         || |
|info       | '' | string | 接口状态说明  |

