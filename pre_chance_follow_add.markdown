### **请求接口**
/index.php?app=Customer&m=MPrechance&a=createRemindChance&access_token=


### **请求方式**
post


### **需要的参数** （必填）
id                                 //为机会id    
plantime                          //跟进时间       1
stage                   （可修改） //跟进结果       5        1 => '初步接洽', '需求确定', '方案/报价', '谈判审核'
follow_rank             （可修改）//调整级别        6    1=>'A(2日内跟进)','B(5日内跟进)','C(7日内跟进)','D(10日内跟进)','E(15日内跟进)'
follow_record                     //跟进记录       8
endtime                          //下次计划时间     9
follow_purpose                   //下次跟进目的       10
follow_method                   //下次跟进方式       11    1=>'电话','接待','拜访','短信','电子邮件','其他'
follow_reason                    //下次跟进理由       12

       

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error  ||返回结果         |
|info       | '' | string | 接口状态说明  |


``` javascript
{
status: 'success',
info: "操作成功"
}
