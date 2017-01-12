# 我的工作流列表
## 请求接口 

> /index.php?app=Workflow&m=IndexApi&a=changenextuser

>  method : post

> *测试http://www.apps.com/index.php?app=Workflow&m=IndexApi&a=changenextuser
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是| 当前登录用户id  |
|id| 是| 当前操作的工作id  |
|checkid| 是| 提交下一审核人的id  |
|mark| 否| 备注  |


## 返回结果

|info|array | array | 返回数据 数组|
|----|----|----|-----|
|statu|0/1 |int|返回状态 1：成功，0：失败|
|info|返回成功失败提示|string|返回提示|

