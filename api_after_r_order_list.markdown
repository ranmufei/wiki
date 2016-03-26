# PublicAfterOrder/get_r_order_list
----
获取维修单列表信息
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
|id	|false| 	int|	        维修单id|	
|r_id   |false|        varchar|	        维修单号|
|fid	|false| 	int|	        返修单id|	
|f_id   |false|	    varchar|	        返修单单号|

## 注意事项
----
参数id ,r_id ,fid,f_id 必填一个



调用样例及调试工具


API测试工具

返回结果
----

## 返回字段说明（基本元数据字段）
----

|返回值字段 |	字段类型	| 字段说明|
|:--|:------|:------------------------:|
|id	|	int|	        维修单id|	
|r_id|	        varchar|	维修单号|
|fid	|	int|	        返修单id|	
|f_id|	varchar|	        返修单单号|
|batchcode|        varchar|        商品条码|
|sarinlcode	|	varchar	|   商品序列号|
|pro_id|	int|	商品id|
|xinhao|	int|	        商品规格id|
|money	|	float|	         价格|
|cl_method|	int|	        处理方式|
|remark|		varchar|	         备注|
