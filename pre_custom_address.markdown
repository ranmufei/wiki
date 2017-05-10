## 客户地址列表
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=list_delivery

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MPrecustom&a=list_delivery&customid=328&access_token=




### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|customid     |客户id | int| `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |{}| {} |看下面示例 |
|info       | '' | string | 接口状态说明  |

``` javascript
{
 count : 1,
 data:[
{
id: "16",
custom_id: "洛克希德马丁",     
receiver: "这是第十一个地址",    //收货人
area: "辽宁省/丹东市/元宝区",    //所在地区
address: "左区的好嘛",          //详细地址
mobile: "1312321221332",       //手机号码
phone: "",                     //固定电话
email: "",                     //邮箱
remark: "",                    //备注
sort: "12",                     //排序
freeze: "0",                
check: "0",
userid: "庆丰包子",              //创建人
createtime: "2015-11-08 16:50",    //创建时间
isdelete: 1                       //是否可删除，1可删，0不可删除
}
 ]
}


### **新增收货地址**
/index.php?app=Customer&m=MPrecustom&a=add_delivery&access_token=   

custom_id:799    //客户id
receiver:呜呜呜   //收货人
area:120115      //所在地区(地址编码)
address:65656565    //详细地址
mobile:1523658965   //联系方式:手机
phone:             //联系方式:电话
email:136@qq.com   //邮箱
remark:的撒旦     //备注