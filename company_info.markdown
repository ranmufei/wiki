# company/info
----
获取公司基本信息
## URL
----
https://1.03in.com/api/v1/company/info
## 支持格式
----
* JSON
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
|XXX	|false	|string|	需要查询的用户昵称。|

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
|:--|:------|:------------------------:|
|cid	|	int64|	公司cID|	
|companyname|	string|	公司名称|	
|company_log|		string|		公司log|	
|company_info	|	string	|	公司简介|	
|company_phone|		int|		公司电话|	
|create_uid|		int|		创认识uid|	
|hanye|		string|		行业|	
|location|		string|		公司地址|	


