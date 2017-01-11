# 我的工作流列表
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=getFormlist

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=getFormlist&p=1&access_token=2c3b84599fcee0081496d827912c4a
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| p| 是 | 分页|


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|count|  | int| 工作流的总数|

|data|array | array | 返回数据 数组|
|----|----|----|-----|
|id| |int|表单id|
|time||varchar|创建时间|
|name|| varchar | 表单名称  |



