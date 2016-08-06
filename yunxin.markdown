# 手机短信/电话   PHP接口

## 说明

  > 发送短信验证码
  > 校验验证码
  > 发送模板短信
  > 查询模板短信发送状态

## 请求方式

   > POST 方式

## 传入参数
 ` type必须传！！
1. 发送短信验证码  type =1   ,  还需传入参数1个： mobile ;  mobile(目标手机号) 
2. 校验验证码     type =2 ，    还需传入参数2个：mobile,code ;  mobile(目标手机号)  , code(验证码) 
3. 发送模板短信  type =3     ， 还需传入参数3个：mobiles,templateid,params; mobiles(接收者号码列表,JSONArray格式,如["186xxxxxxxx","186xxxxxxxx"],最多为100个),templateid(模板编号,netease.im统一后台配置),params(短信参数列表,JSONArray格式，如["xxx","yyy"],依次填充模板)
4. 查询模板短信发送状态  type =4 , 还需传入参数1个：sendid ; sendid(发送短信的编号) 

 ` 注意： 参数不全，会返回错误！！！

## 返回
` 返回Json ，其中code：200（操作成功）、301（被封禁）、315（IP限制）、403（非法操作或没有权限）、404（对象不存在）、413（验证失败(短信服务)）、414（参数错误）、406（频率控制）、500（服务器内部错误）
` 只有 code=200 才是发送成功！
