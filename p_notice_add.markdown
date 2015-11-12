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
| display| 是 |   是否是私有。1、是私有。2、不是私有   |
| chk| 是 |   上传附件的数组（array）   |
| need_id| 否 |   需求的id（如果type==2）   |
| testid| 否 |   测试的id（如果type==4）   |
| sid| 否 |   服务的id（如果type==2）   |
| taskid| 否 |   任务的id（如果type==2）   |
### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|status          |-------   |int    |1.成功。0.失败  |

