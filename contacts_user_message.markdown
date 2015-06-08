### **请求接口**
/index.php?app=Home&m=MobileApi&a=memberInfo

### **请求方式**
get/post

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| memberId     | 是 |   员工id   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|info       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|uid  |              |String |员工id         |
|name        |              |string | 员工姓名         |
|email        |              |String |员工电子邮件  |
|zid     |              |String |员工职位id |
|jid     |              |String |员工部门id |
|phone     |              |String |员工固定电话号码 |
|mobile     |              |String |员工手机号码 |
|postName     |              |String |员工所属职位名称 |
|deptName     |              |String |员工所在部门名称 |

