## 跟进记录
### **请求接口**
/index.php?app=Customer&m=MPrechance&a=record_list


### **请求方式**
get

### **浏览器查看**
http://www.apps.com/index.php?app=Customer&m=MPrechance&a=record_list&themeid=43&access_token=



### **其他参数**
themeid(机会id)


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript

data: {
     count: "1",
     totalPages: 1,
     nowPage: 1,
     data: [{
          id: "42",
          follow_rank: "A",                //原级别    5
          chance_id: "198",  
          createtime: "--",                // 实际跟进时间    2
          follow_record: "--",             //跟进记录        9
          uid: "庆丰包子",                   //操作人员10
          plantime: "0",
          follow_method: "电话",             //跟进方式  3
          stage: "需求确定",                  //跟进结果   4
          follow_reason: "sadsad",                //跟进理由    8
          follow_purpose: "sadsa",              //跟进目的    7
          endtime: "2016-01-27",             // 计划跟进时间  1
          follow_rank_new: "--",             //新级别  6
          avater: "./Uploads/avatar/0/1.jpg"
     }]
}