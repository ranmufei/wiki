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
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript

[
{
id: "66",          //动态ID
title: "",         //动态标题
remark: "我们新",  //动态备注 
origin: "PC端",       //来源(手机端、pc端)
location: "",      //坐标
area: "",          //位置      
userid: "1",       //创建者
createtime: "1436324316",  //创建时间
isdelete: 1                     //1表示可删，0表示不能删除
}
]