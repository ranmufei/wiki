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
stage: "2",             （可修改） //跟进结果    5        1 => '初步接洽', '需求确定', '方案/报价', '谈判审核'
endtime: "2016-01-27",           //计划时间    1
follow_method: "3",              //跟进方式    4    1=>'电话','接待','拜访','短信','电子邮件','其他'
follow_purpose: "sss",           //跟进目的    3
follow_reason: "ssss",           //跟进理由    7
follow_rank: "1",       （可修改）//调整级别    6    1=>'A(2日内跟进)','B(5日内跟进)','C(7日内跟进)','D(10日内跟进)','E(15日内跟进)'
now: "2016-01-28 11:39:02"       //跟进时间    2 
},
status: 1,
info: "查询成功"
}

