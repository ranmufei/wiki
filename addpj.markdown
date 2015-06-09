# 新建票据的上传
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=addpj

>  method : post

## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|uid| 是|用户id|
|money |是|金额|
|file|是|上传图片的数据|
|isreceipt| 是|是否是发票，1为是,2为否|
|documentname| 是|票据名称|
|cateid|  是|类别名称|
|projectid|  是|项目名称|
|docbz|  否|备注|

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|statu|0/1 |int|1表示添加成功，为0表示添加失败|
|info|  |string|提示信息|


``` javascript

html：<input type="file"  id="file">
js：var file = document.getElementById("file").files[0];
