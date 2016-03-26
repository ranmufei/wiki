# company/info
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
|catestate  |false|	int|	需要查询的科目类别， 0代表资产类 1代表负债类 2代表权益类 3代表成本类 4代表损益类。|
|state	|false	|int|	需要查询的科目是否启用的状态。|

## 注意事项
----
参数catestate与state二者必选其一；



调用样例及调试工具


API测试工具

返回结果
----

## 返回字段说明（基本元数据字段）
----

|返回值字段 |	字段类型	| 字段说明|
|:--|:------|:------------------------:|
|id	|	int|	        科目id|	
|code|	        int|	        科目编码|
|name|	varchar|	        科目名称|
|pid|		int|		科目pid|
|path	|	varchar	|	科目path|
|cate|		int|		科目类别|	
|direction|	int|	科目余额方向借/贷|
|analytic|	varchar|	辅助核算|
|amount|	varchar|	核算单位|
|subjectValue|	double|	        科目余额|	