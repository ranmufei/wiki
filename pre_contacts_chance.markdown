## 联系人下机会列表
### **请求接口**
/index.php?app=Customer&m=MPrecontacts&a=chance_list

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrecontacts&a=chance_list&id=46&access_token=

### **公共参数** 
`p` `num`

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |联系人id | string | `*`         |


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
name: "大人",             //机会名称
custom_id: "武汉大学",    //客户名称
stage: "初步接洽",        //机会阶段
createtime: "07-13 17:18",  //创建时间
id: "29"
}
]
},