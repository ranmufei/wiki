### **请求接口**
/index.php?app=Customer&m=MPrechance&a=getChanceRemindDetails&id=201&access_token=



### **请求方式**
get


### **需要的参数**
id                      为机会id     必填


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |1/0  ||返回结果         |
|info       | '' | string | 接口状态说明  |
|data|数据如下 | |   |

``` javascript

{
data: {
id: "201",
stage: "2",                     //跟进结果    5
endtime: "2016-01-27",          //计划时间    1
follow_method: "3",             //跟进方式    4
follow_purpose: "sss",          //跟进目的    3
follow_reason: "ssss",          //跟进理由    7
follow_rank: "1",               //调整级别    6
now: "2016-01-28 11:39:02"      //跟进时间    2 
},
status: 1,
info: "查询成功"
}

