### **请求接口**
/index.php?app=Kaoqin&m=KaoqinApi&a=shenh_power

### **请求方式**
get/post

### **请求参数**

| 参数名称  |必填|     说明      |
|------|-----|------|
| next_uid | 是 |   员工id   |
| cid     | 是 |   公司id   |




### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |1/0/-1 |string |请求状态：  0失败 ； 1成功   |
|info       |成功、失败        |string         |返回结果说明    |
|-----      |-----         |-----  |-----           |





### **列表详细情况 ， 读取JSON数据**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|uid_name | - |string |申请人姓名     |
|creat_time |  2015-01-02 12:00:00     |string   |申请时间    |
|to_time|    2015-01-02 12:00:00       |string | 开始时间         |
|go_time|    2015-01-02 12:00:00       |string | 结束时间         |
|to_time_hour| 5    |string | 预计时间 ，单位是小时  ，注意值包括上班时间，不包括休息时间      |  
|reason|     申请理由         |string |  申请理由 |
|jilu_cate|   申请类型        |string |  申请类型 |
|qj_cate|     请假理由         |string |  请假理由 |
|qj_year|    0        |string |  请假中的年假时长  |
|cc_address|    出差地点        |string | 出差地点 |
