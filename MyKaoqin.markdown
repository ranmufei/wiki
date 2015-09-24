### **请求接口**
/index.php?app=Kaoqin&m=KaoqinApi&a=get_kaoqin_status

### **请求方式**
get/post

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |请求状态         |
|infos       |array         |array  |返回数据 数组    |
|-----      |-----         |-----  |-----           |
|order  |              |int |打卡的序号，第几次打卡         |
|qd_time|              |string | 打卡时间或者“未打卡”         |

