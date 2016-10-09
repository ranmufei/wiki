### **请求接口**
/index.php?app=Comtxl&m=MobileApi&a=phoneBook

### **请求方式**
get

### **公网测试**
http://www.apps.com/index.php?app=Comtxl&m=MobileApi&a=phoneBook

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| departId     | 否 |   部门id   |
| p | 否 |   本接口传入此参数表示分页,不传表示默认第一页 |
| t(暂时未加入) | 是 |   本接口传入此参数表示分页,不传表示默认第一页 |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|uid        |              |String |员工id  |
|name       |              |string |员工姓名   |
|postName   |              |String |员工职位名  |
|avatar|              |String |员工头像  |
|spelling   |              |String |员工姓名拼音全拼(小写) |
|abbreviation |            |String |员工姓名拼音首字母(大写) |
|change	(暂时未加入) |      |boolean|true有修改 ，false没有修改 |

