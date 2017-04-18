## 销售出库订单


 * 获取规格产品的批次
 * @param  [type]  $ckid  仓库id 
 * @param  [type]  $subid 规格id
 * @param  [type]  $str   搜索关键字
 * @param  integer $orderid     订单id
 * @param  integer $p     页码
 * @param  integer $allview     是否显示所有
 * @return [type]         array

## 判断订单是否预约序列号
 - （即销售创建自动入库单  数据表 sale_relate  字段 addinhouse==1）
 -  url ：： app=Invoicimg&m=Batch&a=getformatbatchlist_new&ckid=4&subid=471&orderid=1218&allview=0 
 - jinxiao_batch 中的 ckstatus ==1 表示该批次被全部预约 不可被其他出库单调用  2 部分预约  0 非预约


 