
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