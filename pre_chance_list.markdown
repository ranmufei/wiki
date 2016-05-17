## 销售机会列表
### **请求接口**
/index.php?app=Customer&m=MPrechance&a=lists

### **接口说明**
`分页`

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=lists&id=29sta=1&access_token=

最近7天的跟进计划（无参数）
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=getChanceRemind&access_token=


我请求的战败(get)（status不传参表示查所有，1表示审核中，2表示通过，3表示驳回，数据格式和战败审核一样）

http://www.apps.com/index.php?app=Customer&m=MPrechance&a=applied&access_token=62ce654626ed3e2194de04d77ff892&status=1


-------------------------------------------------


战败审核(NEW)(GET)(status为0是未审核,1为已审核)
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=non_checked&p=1&status=1&access_token=




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
is_leave: "1", （new）         //是否离职  ，1为离职（wangyan（离职））,0为（wangyan）
charge: "wangyan", （new）     //负责人
is_xs: "1"                        //为1就不显示
is_customer: "1"                 //1为线索，0为客户
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
is_leave: "1", （new）         //是否离职  ，1为离职（wangyan（离职））,0为（wangyan）
charge: "wangyan", （new）     //负责人
is_xs: "1"                        //不显示


最近7天的跟进计划（无参数）
{
data: [
{
count: "0",
type: 0,
day: "2016-01-27"
},
{
count: "0",
type: 1,
day: "2016-01-28"
},
{
count: "6",
type: 2,
day: "2016-01-29"
},
{
count: "0",
type: 3,
day: "2016-01-30"
},
{
count: "0",
type: 4,
day: "2016-01-31"
},
{
count: "0",
type: 5,
day: "2016-02-01"
},
{
count: "0",
type: 6,
day: "2016-02-02"
}
],
info: "",
status: "success"
}