### **请求接口**
/index.php?app=Customer&m=MPrethread&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrethread&a=lists&sta=1

/index.php?app=Customer&m=MPrethread&a=commonpower  公海权限为1就显示

{
     xs:1,   //为1显示线索公海

     kh:1    //为1显示客户公海

     isxs:1    //为1显示我的下属
}

### **公共参数** 
`num`、`p`

### **其他参数**
sta  默认不传，当值为1是查询我下属的线索  2为公海线索

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | cname : 客户名称; contact：联系人;  state:状态; createtime:创建时间; post:职务 ; id:ID |
|info       | '' | string | 接口状态说明  |

``` javascript
[
{
cname: "saDSA",
contact: "ASDASd",
mobile: "122345662144",
phone: "1232131231",
post: "",
state: "",
createtime: "11-12 17:16",
id: "453",
is_leave: "1", （new）         //是否离职  ，1为离职（wangyan（离职））,0为（wangyan）
charge: "wangyan", （new）     //负责人
},
……
]