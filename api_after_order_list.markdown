# PublicAfterOrder/get_order_list
----
获取订单列表信息
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
|id|false|	int|	返修单id|
|f_id|false|	varchar|	返修单号|
|o_id|false|	varchar|	 订单单号|
|c_name|false|	varchar|	 客户名|

## 注意事项
----
参数id ,f_id ,o_id,c_name 必填一个



调用样例及调试工具


API测试工具

返回结果
----

## 返回字段说明（基本元数据字段）
----

|返回值字段 |	字段类型	| 字段说明|
|:--|:------|:------------------------:|
|id	|	int|	        返修单id|	
|f_id|	        varchar|	返修单号|
|o_id|	varchar|	        订单单号|
|c_id|		int|		客户cid|
|c_name|        varchar|        客户名|
|lx_tel	|	varchar	|	客户电话|
|lx_address|	varchar	|	客户地址|
|num	|	int|	        商品数量|
|money	|	float|	         价格|
|remark|		varchar|	         备注|
