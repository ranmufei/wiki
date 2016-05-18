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
|count||int|0表示顶级，1表示第二级，以此类推  |

|plist| array |array |项目列表|
|:----|----|----|-----|
|id||int|要传的值|
|projectName||string|在页面显示的项目名称|



### 实例

``` javascript

{
clist: [
{
{
id: "1",
pid: "0",
cateName: "333",
isedit: "0",
default2: "0",
data_edit: "0",
bpath: "0-1",
count: 0

},
{
id: "31",
cateName: "231ggg",
isedit:"0"
default2: "0",
data_edit: "0",
bpath: "0-1",
count:1
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