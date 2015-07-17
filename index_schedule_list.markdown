## 首页 管理管理 今天所有日程
### **请求接口**
/index.php?app=Customer&m=MIndex&a=today_richen

### **接口说明**

### **请求方式**
get

### **浏览器查看**
/index.php?app=Customer&m=MIndex&a=today_richen&access_token=

### **公共参数** 

### **其他参数**
无


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |{}| {} |看下面示例 |
|info       | '' | string | 接口状态说明  |

``` javascript
{
count : 6,
data:[
  {
  id: "188",          //ID
  rid: "188",         //以`id`为准
  title: "我们的世界", //标题
  startime: "2015-07-08 20:11", //开始时间
  uid: "庆丰包子",     //创建人
  createtime: "2015-07-08 20:21"  //创建时间
  }
 ]
}