# 公司考勤打卡请求

> 执行打卡操作

## 请求接口 

>  *index.php?app=Home&m=KaoQingApi&a=daKa*

>  method : get/`post`

> *测试http://www.apps.com/index.php?app=Home&m=KaoQingApi&a=daKa&uid=1&tag=4&address=%E4%B8%8A%E6%B5%B7&cid=1*

## 请求参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
| cid | 否 |   不填安装默认数   |




## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|:----|----|----|-----|
|statu|0/1|int|接口请求状态 有设置时间/无设置时间|
|info|成功/失败|string|状态信息说明|
|:----|---|---|-----|
|data|array|array|时间一维数组 |
|sw_star_time|9:00:00|string|上午上班时间|
|sw_end_time|12:00:00|string|上午下班时间|
|xw_star_time|14:00:00|string|下午上班时间|
|xw_end_time|19:00:00|string|下午下班时间|
|ws_star_time|20:00:00|string|晚上加班上班时间  参考|
|ws_end_time|22:00:00|string|晚上加班下班时间 参考|


