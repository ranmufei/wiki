## 获取线索日程列表
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=view_schedule

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrethread&a=view_schedule&id=331

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
[
{
id: "188",          //ID
rid: "188",         //以`id`为准
title: "我们的世界", //标题
startime: "2015-07-08 20:11", //开始时间
uid: "庆丰包子",     //创建人
createtime: "2015-07-08 20:21"  //创建时间
}
]