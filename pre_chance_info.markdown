## 机会详情
### **请求接口**
/index.php?app=Customer&m=MPrechance&a=view_info

### **接口说明**

### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=view_info&id=29&access_token=

### **公共参数** 

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id     |机会id | string | `*`         |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | {} ||
|info       | '' | string | 接口状态说明  |

``` javascript
{
id: "29",               //ID
name: "大人",           //机会名称
custom_id: "武汉大学",  //所属客户
charge: "庆丰包子",     //负责人
count: "3420000.00",    //销售金额
stage: "初步接洽",      //销售阶段
endtime: "",           //计划时间
remark: "",            //备注
type: "",              //机会类型
source: "",            //机会来源
userid: "庆丰包子",    //创建人
createtime: "07-13 17:18" //创建时间

auditor: "free style",    //审核人     
opertime: "2016-01-27",   //最近操作时间
follow_rank: "A(2日内跟进)",    //跟进级别
auditor_status: "战败申请审核中"   //状态说明    
lose_reason: "质量原因",       //战败主要原因
lose_remark: "",                //战败原因 
fail_remark: "",    
follow_rank_time: "172800",
py: "",                      
py_a: "",   
prolist: [
{
format: "1asf()",    //规格
name: "撒的11",     //产品名称
unitname: "条",     //单位
num: "1",     //数量
id: "49"
}
]
                   








},