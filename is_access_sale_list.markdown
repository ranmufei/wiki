
### **请求接口** 
/index.php?app=Invoicimg&m=SaleMobile&a=is_access_r   是否显示销售单和退货单

/index.php?app=Invoicimg&m=SaleMobile&a=addsalecli      订单两个自定义字段的10条记录


/index.php?app=Invoicimg&m=SaleMobile&a=chiocecustom&status=1&p=1&n=15      
选择客户的列表（

status为1是我的客户 

为2我参与的客户 

为3我下属的客户  

为4我下属参与的客户 

为7所有客户   

p当前页码，n每页的条数）

/index.php?app=Invoicimg&m=SaleMobile&a=custom_address&gsyid=566(通过客户id查询收货地址列表)



### **接口说明**
无需传参数


### **浏览器查看**
http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=addsalecli&access_token=

http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=select_auditlist&apps=&ms=&as=&access_token=

(Customer Chance   autdior)  客户战败

(Sale Index audit)      订单审核

(Sale  Index  SaleCancel)  作废申请

http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=relatesale&p=1&jump=10&gsyid=578   //退货订单关联销售订单的列表

http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=thpr_data&id=5358     //退货订单关联销售订单的产品信息

http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=thxlhlist&id=5358&xinhao=2512&str=   退货关联销售订单的某个型号的序列号（str为搜索字段）


http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=money_cr&id=6   //查询通过汇率id查询汇率

http://www.apps.com/index.php?app=Invoicimg&m=SaleMobile&a=periodlsit&p=1&jump=15&gid=768   //查询周期单（jump 每页显示的条数 p当前查询的页码数 gid客户id）


### **返回结果**


``` javascript
//是否显示
{
statu: 1,    1显示
info: "ok",
data: null
}

{
set: [
0: "自定义",   //订单自定义1的名称
1: "铭牌型号",  //订单自定义2的名称
2: 0,          //订单自定义1是否必填
3: 0,           //订单自定义2是否必填
4: 0,           //订单附件是否必填
5: "工厂fdsf",    //订单产品自定义1的名称
6: "sdf",        //订单产品自定义2的名称
7: "让我儿童",      //订单产品自定义3的名称
8: "1",            //自动创建入库单是否必须勾选
9: 0,              //自动生成序列号按钮是否显示
10: 0,               //订单产品自定义1是否必填
11: 0,              //订单产品自定义2是否必填
12: 0,              //订单产品自定义3是否必填
],
allcussel:1,   //选择客户中（为1所有客户就显示）
openzdyarr: [
{
  sale_def1: "111111"
},
],
openzdyarr2: [
{
   sale_def2: "123.32313"
},
]
cp: 1,    //1为 显示产品订单		
xm: 1,     //1为 显示项目列表
sc: 1,      //1为 自产销售订单
 after: {
       name: "公里数",    //订单产品自定义名称
       is_bt: "0",        //订单产品自定义是否必填
        x_bt: "0"         //订单产品保修期是否必填
 },
wl_isopen: 1   //1为 配件销售订单
}


//客户
{
count: "400",     //总条数
totalPages: 27,    //总页码数
nowPage: 1,    当前页码数
data: [
{
id: "710",                 //客户id
custom_company: "示例客户A 23343 ",    //公司名称
apportion_id: "庆丰包子",          //负责人
custom_type: "",                 //公司类别
online_cid: "0",
pid: "0",
inputtime: "01-03 19:30",       创建时间
type: 0
}
]
}


//审核人
[
{
uid: "619",    //审核人的id
audit: "619",
name: "qwer",    //名称
zname: "班主任",    //职位
img: "./Uploads/avatar/0/619.jpg"   //头像
}
]

//退货订单关联销售订单的列表
{
count: 1,
data: [
{
id: "5358",
uid: "1",
order_num: "XS20161229175127-1",   //销售单号
gys_id: "578",                    
creat_time: "2016-12-29",          //创建时间
count_price: 4560,               //订单金额
ordertype: "2",
from: "自产销售订单",        
ml_price: "0.00",
default6: "5357",
foreign: "",                   //销售货币
gys_name: "紫江企业",          //客户
num: "10.00"                     //订单数量
}
]
}


//退货订单关联销售订单的产品信息
[
{
pro_id: "604",  //产品ud
xinhao: "2204",  //信号id
price: "456.00",   //价格
num: 10,
unit: "596",          //单位id
intoStoreNum: "10.00",   //数量
id: "2204",
name: "星期",         //商品名
format: "haha-4()",     //规格型号
unitname: "瓶",      //单位名称
relation: 1,            //单位换算倍数
sellPrice: "456.00",       //价格
batchss: [   //批次列表
{
id: "776",
intonum: "5",          //出库数量
name: "20161229175310",  //批次名称
formatname: "haha-4",    //规格
productname: "星期",     //产品名称
thnum: 1,               //退货数量
is_thsale: 0
},
{
id: "775",
intonum: "5",
name: "20161229175011",
formatname: "haha-4",
productname: "星期",
thnum: 1,
is_thsale: 0
}
],
xlhdata: {       //序列号列表
count: "1", 
totalPages: 1,
nowPage: 1,
data: [
{
id: "27938",      //序列号id
orderid: "5356",
small_id: "0",
productId: "604",
subTypeId: "2204",
datatime: "2016-12-29 17:45",
type: "33",
storeId: "32",
isShelf: "0",
endtime: "0",
xuliehao: "20161229-116",   //序列号
piciTableId: "775",
mark: null,
default: "1",
default2: null,
ckstatus: "0",
bound: "5358",
intonum: 1,
order_num: "XS20161229175127-1",
sale_order_id: "5358",
batch: "20161229175011",      //批次
product: "星期/haha-4",       //产品/规格
piciname: "20161229175011",
stornhouse: "是是是是",       //出库
disable: true
},

]
},
}
]


{
rate: 8.3183,      //汇率
rate_time: "2017-01-17&nbsp; 09:38:17"
}



//周期单  （某个客户的）

{
count: "1",
totalPages: 1,
nowPage: 1,
data: [
{
id: "64",
number: "JK2017031356485310",   //周期单编号
userid: "1",
customid: "768",
time: "2017-03-13",            //创建时间
startime: "1488988800",
endtime: "1490284800",
orderarr: "6469,6481,6515,6517,6635",
iskp: "1",                          //开票  1为开票 0为不开票
mark: "6666",             //备注
statuskp: "1",
gys_name: "我的是",    //客户
count: 5,             //订单数量
exptime: "2017-03-09~2017-03-24",          //预计结款时间
money: 1573771,         //应收
havePay: 1573771,     //已收金额
kps: {
payMoney: 200,
amount: "20424.00",
periodPercent: "0.9%",
percent: "200,20424.00,0.9%"
},
percent: "200,20424.00,0.9%",      //开票进度（已经开票的额度，总的额度，所占百分比） 已经开票的额度等于0表示尚未开票，总的额度减去已经开票的额度等于0表示开票完成
amount: 1573771,
noPay: 0             //待收金额
}
],
}