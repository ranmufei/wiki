# 用户登录请求

## 请求接口 

### */index.php?app=Core&m=Mclient&a=sypLogin*

>  *请求方式* post

> *开发测试*
  *http://kaifa.linksame.com/index.php?app=Core&m=Mclient&a=sypLogin*

> *公网测试*
  *http://www.apps.com/index.php?app=Core&m=Mclient&a=sypLogin*

## 请求参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| uid | 是 |   当前用户uid   |
| cid | 是 |   当前用户cid  公司id  |
| tag | 否 |   打卡点 1：早上上班；2：早上下班；3 下午上班 ；4 下午下班  |
| address | 是 |   用户地点字符串   |




## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|:----|----|----|-----|
|statu|0/1|int|接口请求状态 失败/成功|
|infos|请求成功|string|状态信息说明|
|nowtime|2013-09-32|date|请求后返回的时间|


