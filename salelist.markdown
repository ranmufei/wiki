### **请求接口**
/index.php?app=Invoicimg&m=SaleMobile&a=mysaleList

### **接口说明**
`分页`

### **请求方式**
get/post

### **浏览器查看（我的销售订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mysaleList&status=1&access_token=

### **浏览器查看（我的退货订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=mysalethList&status=1&access_token=

### **浏览器查看（销售订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=saleList&status=1&access_token=

### **浏览器查看（退货订单）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=salethList&status=1&access_token=


### **浏览器查看（通过大单id查询子单列表）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=get_z_order&id=5357&access_token=   

### **浏览器查看（通过订单id查询详情【订单详情、产品信息、操作日志】）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=info&id=5357&access_token=   

### **浏览器查看（通过订单id查询详情【物流信息】）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=wuliulist&id=5355&access_token=   

### **浏览器查看（通过订单id查询详情【回款信息】）**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=return_list&id=4843&access_token=  


### **公共参数** 
`num`、`p`

### **其他参数**
status     默认传(all)查所有的  2为待确认  1为待审核   3为审核中 0为审核通过     销售订单（  6为订单作废中 7为已作废 8为预计回款 9为我协同的订单（我的销售订单有） 10为已生成序列号订单） 

str        搜索单号或者客户
timestart  筛选的开始时间
timeend    筛选的结束时间 
userid     筛选的员工 （销售订单、退货订单有）


### **返回结果**
|字段       |值             |类型    |说明           |
| --------- |--------|--------|--------       |
|statu| |||
|data |array  |array  | order_num: 销售单号; gys_name：客户; creat_time:创建时间;count_price:订单金额; num:数量; stornstatu:（出库状态/入库状态）; paystatu:（收款状态/退款状态）; from:订单来源（只有我的销售订单和销售订单显示） |
|info| '' | |   |

``` javascript
[
{
count: 0      //没有数据 的情况
data: ""
nowPage: 1
totalPages: 0

}
]


//有数据的情况
[
{
count: "11",
totalPages: 1,
nowPage: 1,
data: [
{
count_price: 1692
creat_time: "2016-01-11"
default6: "0"
from: "产品订单"
gys_id: "386"
gys_name: "uuuuu"
id: "793"
intoStoreNum: "0.00"
is_bigorder: "0"
is_open: 0
is_xs: 0
ml_price: "0.00"
num: "4.00"
order_num: "XS2016111113836 (<span style="color:red">待修改</span>)"
orderstatu: "2"
ordertype: "2"
paystatu: 0
stornstatu: 0
to_address: null
uid: "1"
}
.....
]
}
]

//销售单的
 {
                 key : "order_num",   name : "销售单号", （都有）
                 key : "ordernum" ,     name : "订单号",（都有）
                 key : "gys_name",       name : "客户",（都有）

                 key : "default2", name : "状态",    （8为预计回款） 
                 key : "money",name : "计划回款金额",（8为预计回款）
                 key : "return_time",  name : "回款日期",（8为预计回款）

 		 key : "pro_list" , name : "产品名",  （除了状态8以外的）
                 key : "count_price",name : "订单金额/折扣后总价",（除了状态8以外的）
                 key : "creat_time", name : "创建时间",（除了状态8以外的）
                 key : "to_time", name : "预计交货时间",（除了状态8以外的）
                 key : "num", name : "销售数量",（除了状态8以外的）
                 key : "stornstatu", name : "出库状态",（除了状态8以外的）
                 key : "paystatu",name : "收款状态",（除了状态8以外的）
                 key : "from",name : "订单来源",（除了状态8以外的）
            
            },
//退单的
{
                 key : "order_num", name : "销售退货单号",
                 key : "gys_name",name : "客户",
                 key : "creat_time", name : "创建时间",
                 key : "to_time",name : "预计交货时间",
                 key : "count_price", name : "订单金额",
                 key : "num",name : "退货数量",
                 key : "stornstatu", name : "入库状态",
                 key : "paystatu",  name : "退款状态",
}

//详情
{
		id: "5357",
		uid: "1",
		shenh_uid: "1",
		gys_id: "578",
		order_num: "XS20161229175127",    //销售单号
		creat_time: "16-12-29 17:47",	 //创建时间
		to_time: "1970-01-01",              //交货时间
		count_price: 4560,             //金额
		to_address: "",             //送货地址
		mark: "",                  //备注
		ml_price: "0.00",         //抹零金额：
		orderstatu: "0",
		ordertype: "2",
		default2: "0",
		default3: "1",
		from: "销售订单",             
		isSns: "0",
		default4: "0",
		default5: "s:0:"";", 
		chance_id: "0",    //机会id
		default6: "0",
		is_bigorder: "1",
		ckid_1: "0",
		foreign_currency: "",          //汇率(foreign_currency.money_cr)
		rebate_count: null,           //折后总价
		sale_def1: "",            //订单自定义1的值
		sale_def2: "123.32313",    //订单自定义2的值
		is_use: "0",
		stock_time: null,
		ordernum: "",              //订单号
		sub_audit: 0,
		isadd_thorder: 1,
		is_jq: "199",
		is_addinhouse: "0",
		aftersaleInfo: [ ],
		pici_arr: [ ],
		piciarr: [ ],
		rkbfb: {
		bfb: 0,
		num: 0
		},
		addinhouse: "",
		iskp: "需要开票",    //开票状态
		def1: "工厂",
		def2: "",
		def3: "",
		hkplan: 1,
		ckplan: 1,
		self: 1,
		qcode: "Sale_XS20161229175127",
		parentStatus: 1,
		isself: 0,
		is_cancel: 1,
		audit: 0,          //当前审核人
		liuc: 0,
		sub: 0,
		addressaddress: "",
		jihua_money: 0,
		uname: "庆丰包子",    //创建人员
		ckid: null,
		num: "10.00",          //销售数量或者退货数量
		salefrom: "10",
		ordercates: "自产销售订单",    //订单来源
		gys: "紫江企业",       //客户
		instornNum2: "10.00",
		instornNum: 100,
		kptxmax: 4560,
		kpmoney: "0.00",
		thsale_iszc: 0,
		cws_data: {
		amount: "4560.00",
		pay: "0.00",
		remain: "4560.00",
		opt: "0",
		logs: null
		},
		count_prices: "4560.00",
		havePay: "0.00",          //已付（待付=count_prices-havePay）
		bfb_pay: 0,
		list: [
			{
				id: "8432",
				order_id: "5357", 
				pro_id: "604",
				ctime: "1483004852",
				uid: "1",
				cid: "0",
				name: "",
				b_no: null,
				xinhao: "2204",
				unit: "596",
				price: "456.00",        //销售价
				num: "10.00",          //销售数（以基础单位算的数量）
				intoStoreNum: "10.00",     //已出库
				count_price: "0.00",
				discount: "100",         //折扣（%）
				isdelete: "0",
				supplier_id: null,
				g_time: null,
				title: null,
				price_time: null,
				address: null,
				already_num: "0",
				default1: "0",
				default2: "0",
				wastage: "0",          //产品损耗（以基础单位算的数量）
				thbatch: [ ],
				xlhtitle: null,
				set_id: "0",
				info_id: "0",
				def1: "",
				def2: "",
				def3: "",
				type: "0",
				ispcStatus: "1",
				xlhstatus: "1",
				aftersale: "",
				xuliehao: [
					{
					productId: "604",
					subTypeId: "2204",
					xuliehao: "20161229-124",   //序列号
					formatname: "haha-4",
					proname: "星期"
					},
					{
					productId: "604",
					subTypeId: "2204",
					xuliehao: "20161229-125",
					formatname: "haha-4",
					proname: "星期"
					},
					{
					productId: "604",
					subTypeId: "2204",
					xuliehao: "20161229-126",
					formatname: "haha-4",
					proname: "星期"
					},
					{
					productId: "604",
					subTypeId: "2204",
					xuliehao: "20161229-127",
					formatname: "haha-4",
					proname: "星期"
					},
					{
					productId: "604",
					subTypeId: "2204",
					xuliehao: "20161229-128",   
					formatname: "haha-4",
					proname: "星期"
					}
				],
				proName: "星期",   //产品名称
				formatname: "haha-4()",  //规格或者编码
				_isstatus: 1,
				xuliehaoStatus: 0,
				rk_Status: 1,
				yuyueStatus_xlh: 0,
				yuyueStatus_pc: 0,
				relation: "1",     //单位换算关系
				unitName: "瓶",    //单位
				sum: 10,          //换算单位后的数量
				sum1: 0,         //产品损耗（单位算的数量）
				ketuinum: 0,
				jianqusum: 0,
				baseunitName: "瓶",
				xxnum: 10
			}
		],
			zidan_id: [  //子单产品信息
			{
			id: "5358",
			default5: "山西省/吕梁市/离石区 发展大道158号",   //地址
			is_bigorder: "0",
			data: [
			{
			id: "8433",
			order_id: "5358",
			pro_id: "604",
			ctime: "1483004854",
			uid: "1",
			cid: "0",
			name: "",
			b_no: null,
			xinhao: "2204",
			unit: "596",
			price: "456.00",
			num: "10.00",
			intoStoreNum: "10.00",
			count_price: "0.00",
			discount: "100",
			isdelete: "0",
			supplier_id: null,
			g_time: null,
			title: null,
			price_time: null,
			address: null,
			already_num: "0",
			default1: "1",
			default2: "1",
			wastage: "0",
			thbatch: [ ],
			xlhtitle: null,
			set_id: "0",
			info_id: "0",
			def1: "",
			def2: "",
			def3: "",
			type: "0",
			ispcStatus: "1",
			xlhstatus: "1",
			aftersale: "",
			xuliehao: [ ],
			proName: "星期",
			formatname: "haha-4()",
			_isstatus: 1,
			xuliehaoStatus: 0,
			yuyueStatus_xlh: 0,
			yuyueStatus_pc: 0,
			relation: "1",
			unitName: "瓶",
			sum: 10,
			sum1: 0,
			ketuinum: 0,
			jianqusum: 0,
			baseunitName: "瓶",
			xxnum: 10
			}
			]
			}
		],
		sns: null,
		log: [   //历史记录
		{
		id: "6337",
		orderid: "5357",
		uid: "庆丰包子",           //操作人 
		next_person: "1",
		markLog: "未提交",         //状态
		datatime: "16-12-29 17:47",   //时间
		default: "0",
		default2: "0",
		orderType: "0",
		type: "0",
		avater: "./Uploads/avatar/0/1.jpg",    //头像
		ico: "icon-check"
		},
		{
		id: "6338",
		orderid: "5357",
		uid: "庆丰包子",
		next_person: "0",
		markLog: "已提交",
		datatime: "16-12-29 17:47",
		default: "0",
		default2: "0",
		orderType: "0",
		type: "0",
		avater: "./Uploads/avatar/0/1.jpg",
		ico: "icon-check"
		},
		{
		id: "6339",
		orderid: "5357",
		uid: "庆丰包子",
		next_person: "1",
		markLog: "审核通过",
		datatime: "16-12-29 17:47",
		default: "0",
		default2: "0",
		orderType: "0",
		type: "0",
		avater: "./Uploads/avatar/0/1.jpg",
		ico: "icon-check"
		}
		],
		sale_relate_th: 0,
		sale_def1_text: " ",         //订单自定义1的名称
		sale_def2_text: "铭牌型号",		//订单自定义2的名称
		batchlist: null,
		batchSarial: null,
		choicebatch: null,
		outStronOrder: [ ]
}

//物流
[
{
id: "432",
number: "XS20161229171931-1-1",
order_id: "5355",
sort: "0",
time: "1483005040",
stron_id: "32",
uid: "1",
default: "0",
isDelete: "0",
default2: null,
default3: null,
wl_dynamic: null,
company: null,
express_number: null
},
{
id: "433",
number: "XS20161229171931-1-2",
order_id: "5355",
sort: "1",
time: "1483005137",
stron_id: "32",
uid: "1",
default: "1",
isDelete: "0",
default2: null,
default3: null,
wl_dynamic: [
{
time: "2017-01-01 16:58:04",            //时间
ftime: "2017-01-01 16:58:04", 
context: "[眉山] [眉山市] [眉山]的山南三已收件 电话:13778810535",      //物流动态
location: ""
}
],
company: "中通快递",          //公司(如圆通)
express_number: "424073676174"   //运单号
}
]
