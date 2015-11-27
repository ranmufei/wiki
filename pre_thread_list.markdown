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
|data       |array         |array  | cname : 客户名称; contact：联系人;  state:状态; createtime:创建时间; post:职务 ; id:ID |
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
createtime: "1436324316"  //创建时间
}
]