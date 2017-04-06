# 个人日程列表
## 请求接口 

> /index.php?app=Invoicimg&m=ProductApi&a=getStronOrderByDimension

>  method : post

> http://www.apps.com/index.php?app=Invoicimg&m=ProductApi&a=getStronOrderByDimension&access_token=e133ac84d35628422ca6c2c408667a&dimension=XS201662195242-1
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|dimension| 是 |二维码或者订单号|



###实例
``` javascript

{
order_info: {
id: "2874",
uid: "1",
order_num: "XS201662195242-1",
creat_time: "1466474217",
gys_id: "375",
num: "0",
ordertype: "2",
ckid_1: "0",
ckid_2: "0",
creatTime: "16-06-21 09:56",
username: "庆丰包子",
gysname: "厦门张三"
},
product: [
{
id: "4554",
order_id: "2874",
pro_id: "382",
xinhao: "1051",
unit: "335",
price: "60.00",
num: "2.00",
intoStoreNum: "0.00",
thbatch: "",
proName: "1asdas",
formatname: "9999-9999",
unitname: "夫人"
},
{
id: "4555",
order_id: "2874",
pro_id: "382",
xinhao: "1052",
unit: "335",
price: "30.00",
num: "3.00",
intoStoreNum: "0.00",
thbatch: "",
proName: "1asdas",
formatname: "9999-大号",
unitname: "夫人"
}
],
status: 2
}