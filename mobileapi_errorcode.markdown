### 移动端API 错误码

#### 错误大致分`平台级错误`、`业务错误`

#### 1、平台错误
错误码小于100的调用错误，这种错误一般是由于用户的请求不符合各种基本校验而引起的。目前基本上是授权码错误引起的错误。

| 错误码 |  错误描述-英文  | 错误描述-中文 |  解决方案 |
| :-- | ----:| ----:| :--: |
| 21 | The access token was not found | 缺少access_token参数 | 手机接口的必须参数 |
| 22 | Invalid Format |传递的权限验证参数方式不对 | 如不允许同时在get和post或header中传递access_token |
| 23| Invalid Access Token | 授权码验证失败 |可能是授权码过期或有其他手机登录了该帐号。程序可能重新登录解决问题|

错误返回格式：
<code>
status: "error",
errorCode: 23,
errorDesc: "Invalid Access Token",
info: ""
</code>
