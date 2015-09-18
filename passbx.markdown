# 报销审核
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=passbx

>  method : post

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id |
|id| 是| 报销单id|
|yj| 是| 审核意见|
|status| 是|提交的状态，2为驳回，3为通过,6为下一步审核  |
|audit| 是|选择审核人id  |

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|statu|0/1 |int|1表示审核成功，为0表示审核失败|
|info|  |string|提示信息|