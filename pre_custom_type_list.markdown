## 客户分类列表
### **请求接口**
/index.php?app=Customer&m=MPrecustom&a=get_custom_cat

### **接口说明**

### **请求方式**
get

### **浏览器查看**
www.apps.com/index.php?app=Customer&m=MPrecustom&a=get_custom_cat

### **公共参数** 

### **其他参数**
无


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|data       |看下面示例 | array ||
|info       | '' | string | 接口状态说明  |

``` javascript

[
  {
   id: "1",         //分类ID
   name: "代理商",  //分类名称
   pid: "0",       //分类父级ID
   sort: "0",
   count: 0
  }
 ]
