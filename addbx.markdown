# 报销单的上传接口
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=addbx

>  method : post

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户id |
|audit| 是| 审核人的id |
|name| 是| 报销单名称|
|bxbz| 是| 备注 |
|pjs| 是| 选中的票据数组 |


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|statu|0/1 |int|1表示添加成功，为0表示添加失败|
|info|  |string|提示信息|