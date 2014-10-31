
## 产品详情【读】 :Aries: 

> 产品详情是指产品具体型号列表 包含相关 数量 型号 等。

## 请求接口
 * http://www.apps.com/index.php?app=Home&m=InvoicingApi&a=productInfo&cat_id=77

## 请求参数

|参数名| 必填| 说明|
|:---|----|----|
|cat_id| 是| 产品的id |


## 返回结果
|字段 |  值| 类型 | 说明|
|:----|----|----|-----|
|status| success/error | string| 请求状态 |
|info|array | array | 返回数据 数组|
|id|900|int|产品型号id|
|name|9001*78|string|型号名|
|y_code|JX|string| 产品编码 |
|class_id|12|int|产品大分类别 切记这里的分类是产品大类别 而不是 所属产品名称的那个分类|
|num|903|int|库存数量|
|cat_id|77|int|产品id(产品的id)|
|yujin|0|int|预警下限值|
|content|最新产品处理|string|备注|
|cateName|服装|string|大分类名称|
|proName|新衣服|string |产品名称|

### 返回实例

   ``` javascript

{
status: "success",
info: [
{
id: "24",
name: "100公里*900磅烈性炸药",
y_code: "JX_77_2",
class_id: "54",
num: "234232",
uid: "1",
cat_id: "77",
yujin: "0",
content: ""
},
{
id: "25",
name: "100公里*500磅钻地单",
y_code: "JX_77_3",
class_id: "54",
num: "231",
uid: "1",
cat_id: "77",
yujin: "0",
content: ""
},
{
id: "26",
name: "1000公里*900磅烈性炸药",
y_code: "JX_77_4",
class_id: "54",
num: "430",
uid: "1",
cat_id: "77",
yujin: "0",
content: ""
},
{
id: "27",
name: "1000公里*500磅钻地单",
y_code: "JX_77_5",
class_id: "54",
num: "1233",
uid: "1",
cat_id: "77",
yujin: "0",
content: ""
}
]
}



