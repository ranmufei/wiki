# 公司考勤打卡请求

> 执行打卡操作

## 请求接口 

>  *index.php?app=Kaoqin&m=KaoqinApi&a=daKa*

>  method : get/`post`

> *测试http://www.apps.com/index.php?app=Kaoqin&m=KaoqinApi&a=daKa&uid=1&tag=4&address=%E4%B8%8A%E6%B5%B7&cid=1*

## 请求参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| access_token | 是 |   验证token   |
| uid | 是 |   当前用户uid   |
| cid | 是 |   当前用户cid  公司id  |
| address| 是 |   打卡地址  |
| longitude | 否 |   打卡经度  |
| latitude | 否 |   打卡维度  |
| phone_type| 否 |   手机型号  |



## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|:----|----|----|-----|
|statu|0/1|int|接口请求状态 失败/成功|
|infos|请求成功|string|状态信息说明|
|nowtime|2013-09-32|date|请求后返回的时间|



