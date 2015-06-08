# 用户登录请求

>请求接口

> /index.php?app=Core&m=Mclient&a=sypLogin

> 请求方式 

> post

> 开发测试 

> http://kaifa.linksame.com/index.php?app=Core&m=Mclient&a=sypLogin

> 公网测试  

> http://www.apps.com/index.php?app=Core&m=Mclient&a=sypLogin

## 请求参数

^ 标题一        ^ 标题二       ^ 标题三                 ^
| 第1行，第1列  | 第1行，第2列  | 第1行，第3列           |
| 第2行，第1列  | 合并两栏(注意后面有两个 | 竖号喔)      ||
| 第3行，第1列  | 第3行，第2列  | 第3行，第3列           |
^ 参数名称      ^    必填 ^ 说明  ^
| :-------- | :--------:| :-- |
| user| 是 |   用户登录名   |
| password | 是 |   用户登录密码 |


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|:||||
|errorDesc| |String|错误信息|
|uid|     |string|用户id|
|cid|     |String|用户所在的公司id|
|domain|  |String|用户所在的公司网址|


