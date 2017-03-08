##工作流重新选择审核人

> /index.php?app=Workflow&m=IndexApi&a=answer_work

>  method : get

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=answer_work
## 参数

### **其他参数**
|字段       |说明            |类型    |必填           |
| --------- |--------      |--------|--------       |
|id         |工作id|int|   *|
|checkid    |审核人ID|int|    *|

|mark      |回复信息|string|  |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|statu    |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |