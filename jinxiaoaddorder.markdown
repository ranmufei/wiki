# 添加订单接口

# model('Invoicing')->save_data($data);
## 参数

| 参数名称  |      值|  类型     |说明     |
| :--------  |  ------- | ------| -------- |
|uid     |啊 | string| 啊 |
|order_num     |啊 | string| 订单号 |
|creat_time     |时间戳 | string| 创建时间 |
|to_time     |时间戳 | string| 到货时间 |
|gys_id     |啊 | string| 供应商id |
|num     |啊 | string| 订单总数 |
|count_price     |啊 | string| 订单总价 |
|type     |啊 | string| 0 默认 |
|ordertype     |5 | string| 5：补货出库 |
|form     |2 | string| 分店补货 |
|mark     |啊 | string| 备注 |
|ckid_1     |啊 | string| 出库仓库id  |
## 参数


```` php
$data参数
/**
   *@access [写入] 保存订单数据模型
   *@param $data array 
   *$data[orderinfo]=array('
   *  uid=>
   *  order_num=>
   *  creat_time=>
   *  to_time=>
   *  gys_id=>
   *  num=>
   *  count_price=>
   *  type=> ;'//0/1 本地/网络 订单采购方式'
   *  ordertype=> ;//采购/退货 /销售/退货 0/1 /2/3 5：分店补货
   *  form=> //手动采购/缺货生成采购/分店补货 0/1/2;//
   *  mark=> //备注
   *  ckid_1=>; //选择仓库
   *')   
   *$data['productList']=array(
   *  
   *  pro_id=>
   *  uid=>
   *  xinhao=> '//产品规格id'
   *  price=> ;//采购价
   *  num=> ;//数量
   *  discount= //折扣
   * ) 
   *@return number  成功返回订单id  失败返回 false
   */


````

# 返回 bool  : true/ flase
