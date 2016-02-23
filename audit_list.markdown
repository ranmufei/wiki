# **审核/消息列表**


### **请求接口**
/index.php?app=Home&m=AuditApi&a=getAudit


### **请求方式**
post


### **参数**
| 参数名称  |必填|     说明      |
|------|-----|------|
| uid     | 是 |   员工id   |
| cid     | 是 |   公司id   |
| type     | 是 |   审核类型 ( 1只查看的消息    2业务审批    3办公审批)  |
| status     | 是 |   消息类型 ( -2 : 已读的通知消息 , -1 :未读的通知消息 , 0 : 未审核 , 1 : 已审核 , 2 : 我发起的)  |






## 返回结果
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|status     |-1/0/1/ |string |状态      -1相应参数缺乏 , 1成功 , 0无数据    |
|infos       |状态说明        |string  |状态说明    |
|data       |数组        |array  |返回数组    |


## data类型说明
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|Icon     | string | 应用图片地址  |
|app_name     | string | 应用名称  |
|con_id     | string | 申请原数据id  |
|content     | string | 内容简介  |
|from     | string | 应用的英文名称  |
|from_avatar     | string | 申请人的头像地址  |
|from_name     | string | 申请人的名字  |
|from_uid     | string | 申请人的uid  |
|id     | string | 当前行数据id  |
|is_read     | string | 状态：0未读,1已读,2已审核  |
|stime     | string | 发起时间  |
|title     | string | 申请的标题  |
|type     | string | 类型： 1只查看的消息    2业务审批    3办公审批  |
|checkInfo     | array | 如果是有操作的审核，这里放审核的操作相关数据  |



## checkInfo里面的字段类型说明
|字段       |值             |类型    |说明           |
| --------- |--------      |--------|--------       |
|check_history_url     | string | 获取审核历史记录  |
|check_url     | string | 点击审核同意的post地址  |
|reject_url     | string | 点击驳回同意的post地址  |
|next_check_url     | string | 点击提交下一步审核的post地址  |
|check_history_url     | string | 获取审核历史记录  |
|check_name     | string | 审核按钮的名称 ，默认为“审核”  |
|reject_name     | string | 驳回按钮的名称 ，默认为“驳回”  |
|next_check_name     | string | 提交下一步按钮的名称 ，默认为“提交下一步”  |
|is_reject     | string | 是否有驳回按钮，0代表没有 ， 1代表有  |
|is_next_check     | string | 是否有提交下一步按钮，0代表没有 ， 1代表有  |
|id     | string | 当前记录的id  |
