# 产品列表

# 内部开发调试环境

* 账号登陆授权地址  http://kaifa.linksame.com
* 私有盘测试调用   http://www.apps.com/
* 账号 sving 密码 58456qwe

## 请求地址
*  /index.php?app=Home&m=InvoicingApi&a=productList

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
| p  | 否 |  分页不填安装默认数   |

## 返回说明

| 参数名称  |      值|  类型     |说明     |
| :--------  |  ------- | ------| -------- |
|status     |success/error| string| 接口请求状态码  （成功/失败） 请根据状态值  处理返回数据|

|info       |             | array | 二维数组 |
| :--------  |  ------- | ------| -------- |
|id| | int | 索引编号 |
|uid| | int | 用户id |
|cid| | int | 公司id |
|cat_id| | int | 分类id |
|name| | string| 产品名称 |
|b_no| | sting | 产品编号 |
|unit| | string | 单位 |
|mark| | string | 备注 |
|sns_id| | int | 产品同步到linksame平台的id |




### 实例

``` javascript

{
status: "success",
info: [
{
id: "98",
uid: "1",
cid: "1",
cate_id: "30",
name: "3512354326",
b_no: "346",
xinhao: "346346",
h_id: "346",
unit: "打",
price: "3246.00",
count_price: null,
time: "1405674568",
num: "0",
max_limit: "0",
min_limit: "0",
mark: "62346234",
status: "0",
sns_id: "0"
},
{
id: "97",
uid: "1",
cid: "1",
cate_id: "30",
name: "23452315",
b_no: "1235",
xinhao: "1235",
h_id: "235",
unit: "件",
price: "12351235.00",
count_price: null,
time: "1405674552",
num: "0",
max_limit: "0",
min_limit: "0",
mark: "",
status: "0",
sns_id: "0"
}
}
]
}
