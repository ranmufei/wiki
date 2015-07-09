### 登录

### 说明
在浏览器中完成登录 及跳转到云盘地址进行授权，最后返回授权友等信息

### 返回参数
|字段  |类型  |说明  |
|--------|--------|----- |
|uid     | string |登录者id |
|token   | string | 进行身份认证的授权码 |
|expires | int | token有效期(秒)  |
|refresh_token|string|用来刷新token的验证码|
|refresh_token_expires|int|refresh_token如果连它都失效了，就只能重登了|
|name    | string |登录者名字 |
|domain  | string|云盘地址|
|cid     | int   |登录者所属公司id |
