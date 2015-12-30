### **请求接口**
/index.php?app=Pmanager&m=PmanegerApi&a=get_all_judge
### **公网测试**
http://www.apps.com/index.php?app=Pmanager&m=PmanegerApi&a=get_all_judge&pid=97&cid=1
### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| cid     | 是 |   所在公司id   |
| pid| 是 |  项目的id   |



### **返回结果**
|字段        |值          |类型    |说明        |
| ---------  |--------    |-------- |--------  |
|need_open|-------   |int    |true:开启，false 关闭   |
|test_open| -------     |varchar  |true:开启，false:关闭  |


### **示例**
````php
{
need_open: true,
test_open: false
}