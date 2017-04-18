>接口    url='/index.php?app=Invoicimg&m=Supply&a=outStron_new'

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

> 出库选择批次   
 - 1 预约订单（自产销售订单）  批次的数量 = 预约的序列号总数
 - 2 非预约订单  批次实际数量（可选） = 批次库存总数- 预约数


> 选择序列号  oa_jinxiao_batch_info
 - 1 ckstatus 序列号是否预约 0 非预约 1预约
 - 2 bound    绑定的销售子订单id  0 非绑定  >0 销售子订单id 
 - 3 default  出库状态 0 在库 1 已出库

 