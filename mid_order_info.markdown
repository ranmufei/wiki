## 订单详情
### **请求接口**
/index.php?app=Customer&m=MMidOrder&a=info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MMidOrder&a=info&id=43&access_token=

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
id: "43",            //ID
charge: "庆丰包子",  //负责人
money: "4444.00",   //金额
order_id: "0",      //关联订单ID(不用显示)
custom_id: "dsfadfewredd",   //客户名称
state: "已确认",             //状态 
transform: "0",              //
type: "一次性订单",           //订单类型
endtime: "",                 //结束时间                
remark: "4545454",           //备注
userid: "庆丰包子",          //创建人
inputtime: "2015-07-03 11:02"   //创建时间
},