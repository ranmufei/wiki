### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=share

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=share

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| uid        | 是  |   用户id   |
| file_str   | 是（数组）  |   多个：[1,2,3]   |
| depart_str | 是| 分享到部门|


### **返回结果**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------    |
|status     |success/error  |string  |返回状态    |
|info       |               |array   |返回数据 数组    |
|-----|----|-----|----|
|info|   |string|提示信息|
