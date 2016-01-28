
### **请求接口**
/index.php?app=Customer&m=MPrechance&a=opt_audit&access_token=



### **请求方式**
post


### **需要的参数**
id                      为机会id     必填

type                    类型（2表示通过，3表示驳回，4表示赢单，5表示战败申请） 必填

audit_uid               审核人id(在type=5时必填)

lose_reason             战败申请理由(在type=5时必填)  输入框 

mainLose_reason         战败主要原因(在type=5时必填)  ---- 选项（    1 => '价格原因', '质量原因', '客户关系原因', '其他'   ）


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |success/error |string |返回结果         |
|info       | '' | string | 接口状态说明  |


``` javascript

{
status: "success",
info: "",
}


