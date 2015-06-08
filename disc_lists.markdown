### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=lists

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=lists

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   用户id   |
| folder_id | 否 |   本接口传入此参数表示目录下的文件(夹)列表,不传表示顶级根目录下的文件(夹)列表 |
| page | 是 |   本接口传入此参数表示分页,不传表示默认第一页 |

### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|id         |              |int    |员工id  |
|name       |              |string |员工姓名   |
|size       |              |String |员工职位名  |
|inputtime  |              |int    |员工姓名拼音全拼(小写) |
|file_extension |          |String |员工姓名拼音首字母(大写) |
|type       |              |int    |1=文件 2=文件夹 |
