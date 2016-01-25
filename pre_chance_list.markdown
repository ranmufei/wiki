## 销售机会列表
### **请求接口**
/index.php?app=Customer&m=MPrechance&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=lists&id=29sta=1&access_token=

### **公共参数** 
`p` `num`

### **其他参数**
sta  (1为我参与的，2为我下属的，3为机会提醒（今天），4为机会提醒（逾期），5为战败审核)
timeType（在机会提醒时才会有，0到6）


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
name: "大人",              //机会名称
custom_id: "武汉大学",     //所属客户
stage: "初步接洽",         //阶段
createtime: "07-13 17:18", //创建时间
id: "29"                   //ID
},
]
},


状态为5的data.data

id: "181",
name: "5353",                   //机会名称
custom_id: "uuuuu",              //客户名称
stage: "需求确定",               //销售阶段
auditor: "庆丰包子",             //审核人
createtime: "01-15 11:13",          //创建时间
auditor_status: "战败申请审核中",         //审核状态
lose_reason: ""                           //战败主要原因