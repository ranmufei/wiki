## 客户-联合跟进人
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=share_list&themeid=375&sta=1&num=10&p=1&access_token=

### **接口说明**

### **请求方式**
get


### **其他参数**
p、num
themeid  (关联的id) sta(0为联系人的共享联系人，1为客户的联合跟进人，2为机会的联合跟进人)


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |{}| {} |看下面示例 |
|info       | '' | string | 接口状态说明  |

``` javascript

{
status: "success",
info: "",
data: {
count: "2",
totalPages: 1,
nowPage: 1,
data: [
{
id: "20",
relateid: "谷歌",                      //关联的id   
createtime: "15-12-28 12:06",         //创建时间
userid: "1",                          //创建人
isdelete: 1,                          //1为可删除
avater: "./Uploads/avatar/0/6.jpg"    //头像
}
]
}
}


