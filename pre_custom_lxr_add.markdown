### **请求接口**
/index.php?app=Customer&m=MPrecontacts&a=no_relate_gsy


### **请求方式**
get


### **其他参数**
p、chance（为机会id）


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |             |  array  |   |
|info       | '' | string | 接口状态说明  |


``` javascript
{
data: {
count: "1",
totalPages: 1,
nowPage: 1,
data: [
{
id: "220",
name: "asdfasd",      //姓名
custom_id: "",  
mobile: "",          //手机
sex: "男",           //性别
createtime: "01-22 11:24"   //创建时间
}
]
},
info: "",
status: "success"
}
