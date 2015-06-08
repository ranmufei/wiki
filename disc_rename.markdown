### **请求接口**
/index.php?app=Wangpan&m=MobileApi&a=rename

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Wangpan&m=MobileApi&a=rename

### **请求参数**

| 参数名称   |必填 |     说明   |
|----------- |-----|------------|
| id         | 是  |   文件（夹）唯一id   |
| name   	 | 是  |   文件（夹）重命名   |
| type 		 | 是  |   1=文件 2=文件夹    |


### **返回结果**
|字段       |值             |类型    |说明        |
| --------- |--------       |--------|--------    |
|status     |success/error  |string  |返回状态    |
|info       |               |string  |返回数据 数组    |
|------|--------|------------|------|
|info|  | string| 提示信息|