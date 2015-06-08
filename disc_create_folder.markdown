### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=create_folder

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=create_folder

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| uid        | 是  |   用户id   |
| name       | 是  |   文件夹名称   |
| folder_id  | 否  |   当前目录id,不传表示为0  |


### **返回结果**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------    |
|status     |success/error  |string  |返回状态    |
|info       |               |array| 返回数据 数组   |
|-----      |-----         |-----  |-----           |
|info  |              |String |提示信息         |
