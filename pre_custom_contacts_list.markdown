## 客户下联系人列表
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=contacts_list

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
www.apps.com/index.php?app=Customer&m=MPrecustom&a=contacts_list&id=277

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
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript

{
count: "2",
totalPages: 1,
nowPage: 1,
data: [
{
name: "明明如月天下惊",    //联系人姓名
custom_id: "武汉大学",    //所属客户
sex: "男",               //性别
post: '总经理',          //职位
depart: '部门'           //部门
createtime: "1小时前",   //创建时间
id: "46"                 //ID
},
]
},