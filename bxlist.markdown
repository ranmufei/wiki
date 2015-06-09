# 报销列表
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=pjlist

>  method : get/post

> *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=pjlist&uid=1&status=0
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 用户uid  |
| status| 是 | 当前的票据状态id,不传参默认为0，查询的是所有的|




## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 票据的总数|
|data|array | array | 返回数据 数组|
|:----|----|----|-----|
|id||int|票据id|
