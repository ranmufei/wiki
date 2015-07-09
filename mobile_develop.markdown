### 移动端开发者(android 或 IOS) 请看：

* 身份验证 必须带上 登录时 服务器返回的 验证码，服务器会根据验证码判断出用户身份,所以传不传 用户uid则无关要紧了。不过考虑到对以前 接口的兼容性，是否传uid 请移动端开发者 判断
* 服务器框架对 请求参数 做了兼容性处理,所以一个接口中,参数可以完全POST或GET,程序员不再需要根据 参数 的特性，自己来区分。
* 至于一个接口是POST还是GET请求，这属于业务逻辑的范畴，请移动端工程师 和 服务端 开发者 双方协定。

| 参数名称 |  类型  | 是否必须 |  描述  |
| :-- | ----:| ----:| :--: |
| access_token | string | `*` | 自然是授权码了, 不需要多说 |
| p | int |  | 分页参数 |
| num | int | `*` |每页显示数据条数 默认 25条|


### 服务器端开发者(就是phper) 请看：
- 授权、身份验证什么的，你们就不要管了。这一关我已经控制住了。
- 现在你们的控制器继承的基类是MobileAction(无状态基类)。所以不能用你们以前直接继承Action的方式 去获取框架的一些数据。如 'global $_APP、$this->userinfo'等，请大家注意以下一些事项：
 - 尽量少用(潜台词是不用~_~)全局变量。理由如下：
  - 在Action中$_APP等全局变量，它的数据也是从公共模型获取到的。
  - 全局变量说到底是变量，意思是少写一个字符或多写一个它也不会报错，但对于你来说，就错了。
  - 全局变量要先声明，如果基类换了，如现在是 MobileAction，我没配制全局变量，你调 自然又完了。
  - `总结 直接去查公共模型吧 ，解决所有兼容问题~V~`
- `最后 , 大家有什么问题 , 去公共模型里翻吧！！！`

- 数据的输出用 mobileSuccess、mobileError、ajaxReturn 格式{ data : [] , info : '' , status : 'success' }

- 基类中可用的属性( 调用方式 `$this->xxx` )
 - $uid - 当前登录者
 - $num - 每页显示数据( 当然前期是 该字段 使用公共参数约定`num` )
 - $page - 当前页
- 基类中可用的方法
 - query( $name ) 获取GET参数
 - request( $name ) 获取POST参数
 - server( $name ) 获取$_SERVER参数 
 - mobileResponse( $data , $info='' , $status , $type = 'JSON' )
 - mobileResponse（$data, $info='' , $type='JSON'）
 - mobileError( $data , $info='' , $type="JSON" ) 

