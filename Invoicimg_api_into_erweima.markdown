# 二维码扫描入库接口
## 请求接口 

> /index.php?app=Invoicimg&m=InstockApi&a=inStockOperation

>  method : post

> http://www.apps.com/index.php?app=Invoicimg&m=InstockApi&a=inStockOperation&access_token=e133ac84d35628422ca6c2c408667a
## 参数

| 参数名称  data    |    必填 | 说明  |
| :-------- | :--------:| :-- |
|ckid| 是 |入库的仓库id|
|id| 是 |操作的订单id|
|ordertype| 是 |订单类型|
|mark| 是 |备注|
|piciname| 是 |批次|
|product| 是 |产品数组|


