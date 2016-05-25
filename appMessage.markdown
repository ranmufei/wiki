# 应用消息接口

## 请求接口 

> /index.php?app=Home&m=Audit&a=getNew

>  method : get/post

> *测试http://www.apps.com/index.php?app=Home&m=Audit&a=getNew&from=Account
## 参数

| 参数名称      |    必填 | 说明  |
| :-------- | :--------:| :-- |
|from| 是| 应用名称，如报销Account,考勤Kaoqin |

## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|from| |string|应用名称|
|count||int|新消息的数量|
|menu_id||int|左侧菜单对应的id|


##  说明：
 > 在进入应用时就调用此接口