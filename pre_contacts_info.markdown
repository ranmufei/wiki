## 联系人详情
### **请求接口**
/index.php?app=Customer&m=MPrecontacts&a=view_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrecontacts&a=view_info&id=46&access_token=

### **公共参数** 

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |联系人id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | {} ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
id: "46",                //联系人ID
custom_id: "武汉大学",    //所属客户
charge: "庆丰包子",       //负责人
name: "明明如月天下惊",   //姓名
sex: "男",               //性别
post: "",                //职位
depart: "",              //部门
mobile: "",              //手机
phone: "",               //电话
email: "",               //邮箱
birthday: "",            //生日
address: "",             //地址
hometown: "",            //家乡
age: "",                 //年龄
remark: "",              //备注
userid: "庆丰包子",       //创建人
createtime: "6小时前"     //创建时间
}