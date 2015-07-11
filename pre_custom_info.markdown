## 客户详情
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=view_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrecustom&a=view_info&id=277&access_token=

### **公共参数** 

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |线索id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | {} ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
id: "277",                   //客户ID
userid: "庆丰包子",           //创建者
custom_type: "代理商",        //客户分类 
custom_company: "武汉大学",   //客户名称
level: "",                   //重要等级
pid: "",                     //父级客户名称
url: "",                     //公司网址
scope: "",                   //员工人数
sales: "",                   //年销售额
custom_address: "",          //公司地址  
company_phone: "",           //公司电话 
facsimile: "",               //传真
email: "",                   //公司邮箱 
trade: "",                   //行业
apportion_id: "庆丰包子",     //负责人
remark: "",                  //备注 
inputtime: "2015-07-03 14:56" //创建时间
}