### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=delete

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=delete

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| uid        | 是  |   用户id   |
| file_str   | （二选一）  |   多个：文件集合（1,2,3,4） 单个：1   |
| folder_str | （二选一）  |   多个：文件夹集合（1,2,3,4） 单个：1  |


### **返回结果**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------    |
|status     |success/error  |string  |返回状态    |
|info       |               |string  |提示信息    |
