# treasurer/info
----
获取科目列表信息
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
|cate|false|	varchar|	需要查询的科目辅助核算类别|
|selectid |false	|int|	需要查询的科目自定义辅助核算的id。|

## 注意事项
----
参数catestate与state二者选其一；



调用样例及调试工具


API测试工具

返回结果
----

## 返回字段说明（基本元数据字段）
----

|返回值字段 |	字段类型	| 字段说明|
|:--|:------|:------------------------:|
|id	|	int|	        核算id|	
|ucode|	        int|	        核算编码|
|name|	varchar|	        辅助核算标题|
|standard|	varchar|	核算单位|
|unit    |	varchar	|	核算数量|
|selectid|	int|		新增核算类别|		