私有盘API接口
私有盘针对移动端等便捷查看信息的数据接口,本API接口 HOST 如以 ‘backLinksame’呈现，则表示使用登录时系统返回的host域名。

公共参数列表：
参数名称	是否必须	说明
uid	视接口而定	当前登录者Id
p	视接口而定	分页参数名
num	视接口而定	系统默认为10，如果开发者想更改则传入此参数
以下接口涉及公共参数将不做说明。
获取公司部门
请求语法:
GET 	/index.php?app=Home&m=MobileApi&a=departments
HOST:  backLinksame
接口参数:	无

通讯录
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=phoneBook
HOST:  backLinksame
接口参数:
参数名称	必填	说明
departId	否	部门Id
p	否	本接口传入此参数表示分页,不传表示不分页。

返回数据信息
参数	值类型	说明 
uid		int	职员id
name	String	员工姓名
postName	String	职位名

员工详情
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=memberInfo
HOST:  backLinksame
接口参数

参数名称	必填	说明
memberId	是	职员Id

返回数据信息
参数	值类型	说明 
uid		int	职员id
name	String	员工姓名
email	String	电子邮件
zid	int	职位id
jid	int	部门id
phone	string	电话
mobile	string	手机
postName	string	职位名
deptName	string	部门名


通知公告
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=notice
HOST:  backLinksame
接口参数
参数名称	必填	说明
uid	是	
p	是	

返回数据信息
参数	值类型	说明 
id		int	公告id
title		String	公告标题
inputtime	String	创建时间
valid	int	0:过期 1:有效期限

公告详情
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=noticeInfo
HOST:  backLinksame
接口参数
参数名称	必填	说明
id	是	公告id
uid	是	

返回数据信息
参数	值类型	说明 
id		int	公告id
title		String	公告标题
limits	String	权限范围
inputtime	String	创建时间
outtime	String	过期时间
content	String	公告详情

客户全部类型
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customTypes
HOST:  backLinksame
接口参数	无

员工客户列表
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customers
HOST:  backLinksame
接口参数
	
参数名称	必填	说明
typeId	否	客户类型Id
p	是	
uid		是	员工id

返回数据信息
参数	值类型	说明 
id		int	客户 id
custom_type		int	客户类型
custom_company	String	公司名
mobile	String	联系方式

公共客户列表
接口参数
	
参数名称	必填	说明
p	是	

返回数据信息
参数	值类型	说明 
id		int	客户 id
custom_type		int	客户类型
custom_company	String	公司名
mobile	String	联系方式

客户详情
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customInfo
HOST:  backLinksame
接口参数
参数名称	必填	说明
id	是	客户id
uid	是	

返回数据信息
参数	值类型	说明 
id		int	客户 id
custom_type	int	客户类型
custom_company	String	公司名
custom_name	String	联系人
is_company	Int	0私有客户 1公共客户
post	String	职位
custom_address	String	公司地址
mobile	String	联系电话
zipcode	String	邮编
company_phone	String	公司电话
facsimile	String	传真
email	String	电子邮件
trade	Int	行业Id
remark	String	备注
inputtime	String	创建时间
custom_type_name	String	客户类型
trade_name	String	行业名称

销售机会列表（客户管理）
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customChances
HOST:  backLinksame
接口参数
参数名称	必填	说明	
uid	是	
p	是	

返回数据信息
参数	值类型	说明 
id		int	销售机会 id
custom_id	int	客户id
chance_stage	String	目前状态
custom_company	String	公司名


销售机会详情（客户管理）
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customChanceInfo
HOST:  backLinksame
接口参数
参数名称	必填	说明	
id	是	销售机会Id
uid	是	

返回参数说明
参数	值类型	说明 
custom_id	int	客户id
chance_form	String	销售机会来源
sell_stage	String	销售阶段
expect_money	Float	预计金额
possibility	String	成功可能性
chance_stage	String	机会状态
outtime	String	预计结束时间
remark	String	备注
custom_company	String	公司名称
importStr	String	重要程度


联系计划列表（客户管理）
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customTouchs
HOST:  backLinksame
接口参数
参数名称	必填	说明	
uid	是	

返回数据信息
参数	值类型	说明 
id		int	联系计划 id
custom_id	int	客户id
title	String	联系计划主题
custom_company	String	公司名

联系计划详情（客户管理）
请求语法
GET 	/index.php?app=Home&m=MobileApi&a=customTouchInfo
HOST:  backLinksame
接口参数
参数名称	必填	说明	
id	是	联系计划Id
uid	是	

返回参数说明
参数	值类型	说明 
custom_id	int	客户id
touch_type	String	联系原因
title	String	联系主题
plan_time	touch_way	联系时间
touch_way	String	联系方式
inputtime	String	创建时间
remark	String	备注
custom_company	String	公司名称

联系计划 全部更新记录
请求语法 
GET 	/index.php?app=Home&m=MobileApi&a=getCustomTouchNotes
HOST:  backLinksame
接口参数
参数名称	必填	说明	
touchId	是	联系计划Id

返回参数说明
参数	值类型	说明 
remark	String	备注
inputtime	String	创建时间
location	String	地理位置

销售机会 全部更新记录
请求语法 
GET 	/index.php?app=Home&m=MobileApi&a=getCustomChanceNotes
HOST:  backLinksame
接口参数
参数名称	必填	说明	
touchId	是	销售机会Id

返回参数说明
参数	值类型	说明 
remark	String	备注
inputtime	String	创建时间


销售机会 更新记录操作





















日程
接口说明
（1）获取今天 以及 今天以后的日程数据 列表


请求
Get 		/index.php?app=Home&m=MobileApi&a=myRichen
返回类型json  


接口参数
参数名称	必填	说明	
uid	是	用户的uid
p	否	分页（第几页）
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
uid		int	
cid		int	公司id
creattime			日程开始时间
endtime			日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title		string	日程标题
content			日程内容
tixintime			提前提醒时间
status			



（2）获取我的所有个人日程列表


请求
Get 		/index.php?app=Home&m=MobileApi&a=myAllRichen
返回类型json  


接口参数
参数名称	必填	说明	
uid	是	用户的uid
p	否	分页（第几页）
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
uid		int	
cid		int	公司id
creattime			日程开始时间
endtime			日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title		string	日程标题
content			日程内容
tixintime			提前提醒时间
status			










（3）读取具体日程


请求
Get 		/index.php?app=Home&m=MobileApi&a=richenInfo
返回类型json  


接口参数
参数名称	必填	说明	
uid	是	用户的uid
rid	是	日程id
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
uid		int	
cid		int	公司id
creattime			日程开始时间
endtime			日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title		string	日程标题
content			日程内容
tixintime			提前提醒时间
status			
comment		array	该日程的评论
id		int	评论id
r_id			日程id
comment		string	评论内容
time		num	评论时间


（4）受邀日程列表

请求
1当天受邀

Get 		/index.php?app=Home&m=MobileApi&a=byYaoqin   



返回类型json  


接口参数
参数名称	必填	说明	
		
		
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
uid		int	
cid		int	公司id
creattime			日程开始时间
endtime			日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title		string	日程标题
content			日程内容
tixintime			提前提醒时间
status			
			
			
			
			
			


（5）受邀日程列表

请求

全部受邀

Get      /  index.php?app=Home&m=MobileApi&a=byAllYaoqin

返回类型json  


接口参数
参数名称	必填	说明	
		
		
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
uid		int	
cid		int	公司id
creattime			日程开始时间
endtime			日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title		string	日程标题
content			日程内容
tixintime			提前提醒时间
status			
			
			
			
			
			



（6）添加日程

请求
post		/index.php?app=Home&m=MobileApi&a=richenCreat

返回类型json  
{
Status:success //成功 error表示失败
Info:{
Statu:0,
Info:请求成功
}
}

请求字段说明

参数名称	必填	类型	说明	
			
			
uid	Y	int	
cid	YY	int	公司id
creattime	Y		日程开始时间
endtime	Y		日程结束时间
type	0/1	int	个人日程/公司日程
important	0-5	int	日程重要等级1-5 值越大越重要
title	Y	string	日程标题
content	Y		日程内容
tixintime	N		提前提醒时间
status	N		
usertype	N	string	被邀请人的uid 字符串 例如（“11,32,43,”）多人用逗号分隔开
			
			
			
			




工作流

（1）我的全部工作流


请求
Get 		/index.php?app=Home&m=MobileApi&a=workflowAll
返回类型json  


接口参数
参数名称	必填	说明	
uid	是	用户的uid
p	是	分页数
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
Text_id		int	存放内容表id
description		text	工作描述
lcid			流程id
uid			用户id
cid	0/1	int	自己公司id
endtime	0-5	int	结束时间
status	0/1	string	0 进行中/ 1结束
time			创建时间
			
			
			
			
			
			
			




（2）我的待处理任务
请求
Get 		/index.php?app=Home&m=MobileApi&a=workMyTask
返回类型json  


接口参数
参数名称	必填	说明	
uid	是	用户的uid
p		分页数
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
Text_id		int	存放内容表id
description		text	工作描述
lcid			流程id
uid			用户id
cid	0/1	int	自己公司id
endtime	0-5	int	结束时间
status	0/1	string	0 进行中/ 1结束
time			创建时间
			
			
			
			
			
			
			




（3）工作流详情
请求
Get 		/index.php?app=Home&m=MobileApi&a=workflowInfo
返回类型json  

测试参考
http://www.apps.com/index.php?app=Home&m=MobileApi&a=workflowInfo&wkid=21




接口参数
参数名称	必填	说明	
uid	是	用户的uid
p		分页数
返回说明

参数名称	值	类型	说明	
status	success	string	请求成功
Info		array	请求成功后返回的值
id		int	编号id
Text_id		int	存放内容表id
description		text	工作描述
lcid			流程id
uid			用户id
cid	0/1	int	自己公司id
endtime	0-5	int	结束时间
status	0/1	string	0 进行中/ 1结束
time			创建时间
			
			
history		array	审核记录
id			审核记录id
wk_id		int	工作id
bz_id		int	
mark		text	审核内容
uid			审核人id
Creat_time			审核时间
			
dshid		int	当前工作流等待谁审核
dshid			待审核人id
d_name			名字
table			审核表单中的内容
cont			表单字段的内容
type			备注说明
ziduan			字段名


（4） 审核工作流
请求
Get 		/index.php?app=Home&m=MobileApi&a=workflowShenh
返回类型json  

接口参数
参数名称	必填	说明	
wkid	是	工作id
mark	是	提交审核内容
usertype	否	选择的审核人
uid		uid
返回说明
参数名称	value	说明	
status	success/error	接口请求结果 
info	是	提交审核内容
statu	1/0	成功/失败
info		说明文字

（5） 发送催促
请求
Get 		/index.php?app=Home&m=MobileApi&a=workflowSendC
返回类型json  

接口参数
参数名称	必填	说明	
wkid	是	工作id
		
		
返回说明
参数名称	value	说明	
status	success/error	接口请求结果 
info		提交审核内容
statu	1/0	成功/失败
info		说明文字





（6）操作记录
请求
Get 		/index.php?app=Home&m=MobileApi&a=workHistory
返回类型json  

接口参数
参数名称	必填	说明	
uid	是	uid
p	否	分页（默认25）
		
返回说明
参数名称	value	说明	
status	success/error	接口请求结果 
info		提交审核内容
id	1/0	当前记录id
wk_id		工作id
bz_id		
mark		备注
creat_time		操作时间
uid		用户uid (自己)


