## 客户动态列表
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=view_dynamics

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrecustom&a=view_dynamics&id=277&access_token=
### **公共参数** 
`p` `num`

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |客户id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array | count:总数据量 , totalPages:总页数 ， nowPage:当前页 , data:[]数据列表(具体查看以下代码)|
|info       | '' | string | 接口状态说明  |

``` javascript

data: [
{
id: "67",               //客户ID
title: "",             
remark: "樱花纷飞之里",  //备注
origin: "PC端",         //来源
location: "",           //坐标 
area: "",               //地址
userid: "庆丰包子",      //创建者
createtime: "10:40"     //创建时间
}
]