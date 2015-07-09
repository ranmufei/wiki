## 获取线索详情
### **请求接口**
/index.php?app=Customer&m=MPrethread&a=view_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrethread&a=view_info&id=331

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
{
id: "331",               //线索ID
charge: "庆丰包子",      //负责人 
cname: "武汉科技大学",   //客户名称
contact: "江丽",        //联系人
state: "已联系",        //状态
sex: "男",              //性别 
depart: "信息化研究部",  //部门
post: "经理",           //职位
phone: "3131313131",    //电话
mobile: "1313131313",   //手机
email: "",              //邮箱
weibo: "",              //微博
area: "",               //地区
address: "",            //详细地址
code: "",               //邮编
source: "",             //线索来源
remark: "",             //备注
userid: "庆丰包子",      //创建人
createtime: "06-26 11:26",  //创建时间
}