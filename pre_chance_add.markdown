### **新增销售机会**

### **请求接口**
/index.php?app=Customer&m=MPrechance&a=add_chance

### **接口说明**

### **请求方式**
post

### **浏览器查看**
无

### **公共参数** 
无

### **其他参数**
|字段       |说明            |表单类型|表单补充    |必填           |
| --------- |--------      |--------|------- |--------       |
|name      |机会名称   |输入框 | | `*`         |
|custom_id |所属客户 |选择 |[查询客户](http://192.168.1.240/ranmufei/apps/wikis/pre_custom_search_like) | `*` |
|count     |销售金额 |输入框 |||
|stage     |销售阶段 |选项 | 1-初步接洽 2-需求确定 3-方案/报价 4-谈判审核 (5-赢单 6-输单 不显示) | `*` |
|endtime   |下次跟进时间|日期 | | `*`    |
|type      |机会类型 |选项 | 1-新客户机会 2-老客户机会 ||
|source    |机会来源 |选项 | 1-广告 2-研讨会 3-搜索引擎 4-客户介绍 5-其他 | |
|remark    |备注     |输入框| | |
|follow_rank|跟进级别|选项 |1=>'A(2日内跟进)','B(5日内跟进)','C(7日内跟进)','D(10日内跟进)','E(15日内跟进)' |  `*`   |
|follow_method|计划跟进方式|选项 | 1=>'电话','接待','拜访','短信','电子邮件','其他' | `*`    |
|follow_purpose|计划跟进目的|输入框| |  `*`   |
|follow_reason|下次跟进理由|输入框| | `*`    |
|is_customer| 0为客户，1为线索|int || `*`|
|prolist| 产品数组|array |[产品列表](http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getFormatList&access_token=2c3b84599fcee0081496d827912c4a)|[是否必填](http://www.apps.com/index.php?app=Customer&m=MPrechance&a=is_btpro&access_token=2c3b84599fcee0081496d827912c4a)|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |array         |array  | |
|info       | '' | string | 接口状态说明  |

``` javascript

prolist[0][id]:2375    // 产品型号
prolist[0][proid]:657  // 产品id
prolist[0][name]:撒的11
prolist[0][format]:1asf
prolist[0][num]:1        //数量
prolist[0][unit]:653
prolist[0][unitname]:条


