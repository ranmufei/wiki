# 类别、项目列表
## 请求接口 

> /index.php?app=Account&m=ExpenseApi&a=pclist

>  method : get
>  *测试http://www.apps.com/index.php?app=Account&m=ExpenseApi&a=pclist

## 参数（无须传参）

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|

||array |array |类别列表|
|:----|----|----|-----|
|pro_name||string|项目名称|
|percent||string|项目进度|
|leader||string|项目创建人|
|time||string|项目创建时间|

### 实例

``` javascript

{
count: "1",
totalPages: 1,
nowPage: 1,
html: "<ul><li> <li class='active'><a href='javascript:' >1</a></li><li><a href='/index.php?m=ExpenseApi&a=get_pmanager_list&app=Account&access_token=255f44d883c50dc0ef190c2ed51a31&p=2'>2</a></li><li><a href='/index.php?m=ExpenseApi&a=get_pmanager_list&app=Account&access_token=255f44d883c50dc0ef190c2ed51a31&p=3'>3</a></li><li><a href='/index.php?m=ExpenseApi&a=get_pmanager_list&app=Account&access_token=255f44d883c50dc0ef190c2ed51a31&p=4'>4</a></li> <li><a href='/index.php?m=ExpenseApi&a=get_pmanager_list&app=Account&access_token=255f44d883c50dc0ef190c2ed51a31&p=2'>下一页</a></li> &nbsp;&nbsp;NUM:94 1/4 页</li></ul>",
data: [
{
id: "158",
uid: "庆丰包子",
cid: "1",
pro_name: "9999",
objective: "999999",
time: "2015-12-03",
end_time: "2015-12-11",
leader: "庆丰包子",
user: ",78,361,385,388",
display: "0",
status: "0",
isOrder: "0",
percent: "0%"
}
]
}