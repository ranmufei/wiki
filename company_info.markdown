# users/show
----
根据用户ID获取用户信息
## URL
----
https://api.weibo.com/2/users/show.json
## 支持格式
----
*JSON
## HTTP请求方式
----
GET
## 是否需要登录
----
*是
关于登录授权，参见 如何登录授权
## 访问授权限制
----
访问级别：普通接口

频次限制：是

关于频次限制，参见 接口访问权限说明

## 请求参数
----
|| 	必选	|类型及范围	|说明|
|:---|:--|:--|:--|
|access_token	|true|	string	|采用OAuth授权方式为必填参数，OAuth授权后获得。|
|uid	|false|	int64|	需要查询的用户ID。|
|screen_name	|false	|string|	需要查询的用户昵称。|

## 注意事项
----
参数uid与screen_name二者必选其一，且只能选其一；

接口升级后，对未授权本应用的uid，将无法获取其个人简介、认证原因、粉丝数、关注数、微博数及最近一条微博内容。

调用样例及调试工具


API测试工具

返回结果
----

## 返回字段说明
----

|返回值字段 |	字段类型	| 字段说明|
|id	|	int64	用户UID|	
|idstr	|	string|		字符串型的用户UID|	
|screen_name|		string|		用户昵称|	
|name	|	string	|	友好显示名称|	
|province|		int|		用户所在省级ID|	
|city|		int|		用户所在城市ID|	
|location|		string|		用户所在地|	
|description|		string|		用户个人描述|	
|url|		string|		用户博客地址|	
|profile_image_url|		string	用户头像地址（中图），50×50像素|	

