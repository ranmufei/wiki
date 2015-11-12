### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=uploads_call
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=uploads_call
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |
| uid| 是 |  使用人的id   |

### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|all_name          |-------   |varchar    | 上传文件的全名  |
|attid| -------     |int  |  附件存放表id    |
|info| -------    |varchar  |附件上传路径   |
|name| -------     |varchar  |缩略文件名   |



