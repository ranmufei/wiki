### **我的客户列表**

### **请求接口**
/index.php?app=Customer&m=MLegwork&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MLegwork&a=lists&sta=1&access_token=
### **公共参数** 
`num`、`p`

### **其他参数**
`sta`（1外勤签到详单,2客户拜访统计,3效能统计）

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|data       |array         |array  | count:总数据量 , totalPages:总页数 ， nowPage:当前页 , data:[]数据列表(具体查看以下代码) |
|info       | '' | string | 接口状态说明  |

``` javascript
data: [
{
userid: "庆丰包子",                            //员工
time: "2016-01-18 17:32",                     //签到时间
address: "湖北省 武汉市 汉阳区 龟山北路 8号",   //签到地址
gsy_id: "uuuuu",                               //客户
contacts_id: "youting123_lxr1111",              //联系人
mark: "网哈萨克在",                                //备注
lng: "114.274156",
lat: "30.561943",
range: "正常-569米"                               // 签到距离      
}
]


********客户拜访统计**********
data: [
{
id: "349",
custom_company: "asDsdsad",       //客户
custom_address: "",               //客户地址
apportion_id: "庆丰包子",          //   负责人
lng: "",                       
lat: "",
count_rang: 0,                      //拜访次数
user_count: 0                      //距离异常次数
}
]

*********效能统计**********
data: [
{
uid: "254",                  
name: "324234",             //员工
jid: "无部门",              //部门
count: "0",                //签到次数
gsy_legwork: "0",         //客户拜访次数
gsysum: "0",             //客户总量
bfkhl: 0                //拜访客户量
}
]