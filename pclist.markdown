# 类别、项目列表
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=pclist

>  method : get
>  *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=pclist

## 参数（无须传参）

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|

|clist|array |array |类别列表|
|:----|----|----|-----|
|id||int|要传的值|
|cateName||string|在页面显示的类别名称|
|isedit||int|等于1时只能看不能选  |

|plist| array |array |项目列表|
|:----|----|----|-----|
|id||int|要传的值|
|projectName||string|在页面显示的项目名称|



### 实例

``` javascript

{
clist: [
{
id: "2",
cateName: "办公用品",
isdelete: "0",
default1: "",
default2: ""
},
{
id: "31",
cateName: "231ggg",
isdelete: "0",
default1: "",
default2: ""
}
],
plist: [
{
id: "4",
projectName: "项目2",
isdelete: "0",
default1: "",
default2: ""
},
{
id: "5",
projectName: "项目w",
isdelete: "0",
default1: "",
default2: ""
}
]
}