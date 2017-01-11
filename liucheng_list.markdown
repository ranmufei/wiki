# 我的工作流列表
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=getliuchengList

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=getliuchengList&p=1&access_token=2c3b84599fcee0081496d827912c4a
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
|id| |int|流程id|
|lc_name||varchar|流程名称|
|description||varchar|流程描述|
|fm|| varchar | 表单名称  |



