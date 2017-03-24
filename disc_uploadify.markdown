### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=uploadify

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=uploadify

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| uid        | 是  |   用户id   |
| fid  | 否  |   本接口传入此参数表示目录id,不传表示默认为0  |
| file  | 是  |   本接口传入此参数表示上传文件信息  |


### **返回结果**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------   |
|status     |success/error  |string  |返回状态    |
|info       |               |array  |    |
|---------| | | |
|tips| | string | 提示文字  |