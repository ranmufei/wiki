现金流 对 其他应用 提供现金交易 及 订单 审核 的功能接口。
### _分为两步_：
- 创建对应来源的现金流规格对象( model('CashFlow') )
  -- 在线报销付款 createExpensePay()
  -- 样品出借收款 createSampleLoan()
  -- 连锁收银收款 createSyCollect()
- 通过第一步的现金流规格对象调用统一的接口实现现金流的各种操作

新增 现金流
![QQ截图20150526152827](http://192.168.1.240/uploads/ranmufei/apps/7014d2b354/QQ%E6%88%AA%E5%9B%BE20150526152827.png)

查看现金流 支付 记录
 ![QQ截图20150526160759](http://192.168.1.240/uploads/ranmufei/apps/57777815be/QQ%E6%88%AA%E5%9B%BE20150526160759.png)

| 参数名称  |     类型|说明|
|:-------- | ------| -------- |
|amount| string| 现金流总金额|
|pay| string| 已付 |
|remain| string | 未付 |
|onInit| function| null | 组件初始化后的回调 |
|opt | int | 付款/收款(暂时不需要) |
|logs| array[ 'amount'/*金额*/ , 'inputtime'/*时间*/ , 'username'/*操作人*/ ] | 付款记录  | 