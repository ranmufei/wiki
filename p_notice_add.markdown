### **请求接口**
/index.php?app=Barcode&m=PmanegerApi&a=addnotice



### **公网测试**
http://www.apps.com/index.php?app=Barcode&m=PmanegerApi&a=addnotice

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid| 是 |   用户id  |
| cid| 是 | 用户公司id  |
| notice| 是 |   动态信息  |
| type| 是 |动态内容---- 1:主页动态 2：需求动态给need_id（必须） 3：项目动态 4 测试动态给test_id（必须） 5 服务动态server_id（必须） 6任务动态给server_id（必须）    |
| returntime| 是 |   归还时间   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|chuqin          |-------   |int    |出勤比例  |
|weichuqin      | -------     |int    |未出勤比例      |
### **示例**
````php
{
chuqin: 0,
weichuqin: 100
}