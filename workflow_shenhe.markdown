# 工作审核
##工作协同同意审核 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=agree_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=agree_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|uid         |用户ID|int|    *|
|mark         |回复信息|string|   必传（单用户可写可不写）|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |



##工作协同不同意审核 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=disagree_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=disagree_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|uid         |用户ID|int|    *|
|mark         |回复信息|string|   必传|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |



##工作终审同意审核 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=pass_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=pass_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|uid         |用户ID|int|    *|
|mark         |回复信息|string|   必传|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |



##工作终审不通过 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=reject_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=reject_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|uid         |用户ID|int|    *|
|mark         |回复信息|string|   必传|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |


##工作终审通过回复意见 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=answer_work

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=answer_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|uid         |用户ID|int|    *|
|mark         |回复信息|string|   必传|

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |