# Linksame调用手机短信接口

>  model('Sms')->index($type,$sendArr) ; 

> /*
>        * type必须传！！

>        * 发送短信验证码 type =1 , 还需传入参数1个： mobile ; mobile(目标手机号)

>        * 校验验证码 type =2 ， 还需传入参数2个：mobile,code ; mobile(目标手机号) , code(验证码)
>        * 发送模板短信 type =3 ， 还需传入参数3个：mobiles,templateid,params; mobiles(接收者号码列表,JSONArray格式,如   ["186xxxxxxxx","186xxxxxxxx"],最多为100个),
> templateid(模板编号,netease.im统一后台配置),params(短信参数列表,JSONArray格式，如["xxx","yyy"],依次填充模板)
>       * 查询模板短信发送状态 type =4 , 还需传入参数1个：sendid ; sendid(发送短信的编号)
>         * $sendArr 包含cid,uid,mobile,mobiles,code,templateid,params，对应type不一样，参数不一样；
>         ` 注意： 参数不全，会返回错误！！！
> */

## 已审核通过的templateid列表
| templateid   | 名称   | 通过时间  | 短信模板  |
| :--  | ----:| :--: | :--: |
| 3034018  | 项目管理有新通知 | 2016-08-05 17:13:57 | %s项目，邀你共同参与。%s，项目负责人：%s，开始时间：%s，结束时间%s，当前进度：%s。 |

## 返回
` 返回Json ，其中code：200（操作成功）、301（被封禁）、315（IP限制）、403（非法操作或没有权限）、404（对象不存在）、413（验证失败(短信服务)）、414（参数错误）、406（频率控制）、500（服务器内部错误）
` 只有 code=200 才是发送成功！

## 注意

   >  如果返回  414参数错误  ，请检查参数是否带全，以及参数中不能出现 %s 字眼！！！！！！！！！！！！！！！！
