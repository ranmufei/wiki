## 数据处理 model('Excel')->importExcel($path); //导入数据处理

-$value[0];//商品名称
-$value[1];//规格一
-$value[2];//规格二
-$value[3];//多规格/单品
-$value[4];//产品编码
-$value[5];//规格编码
-$value[6];//母件编码
-$value[7];//物料编码
-$value[8];//物料名称
-$value[9];//分类
-$value[10];//成本价
-$value[11];//销售价
-$value[12];//供应商编码
-$value[13];//单位
-$value[14];//品牌
-$value[15];//备注
-$value[16];//数量
-$value[17];//损耗
-$value[18];//自产
-$value[19];//批次
-$value[20];//序列号
-$value[21];//初始化仓库
-$value[22];//库存数量


##产品添加
-（判断 $value[0]'商品名称'，$value[4]'产品编码'，$value[5]'规格编码' 都存在 ）
##物料添加
-（判断 $value[0]'商品名称'，$value[4]'产品编码'，$value[5]'规格编码' 不存在 ）


##产品bom结构的构建
-根据  $value[6];//母件编码在  导入的数组中 检索对应的物料数组  D('ProductInfo')->getRightArray($value[5]/规格编码 ,$getarry,6); 

##物料bom结构的构建
-根据  $value[6];//母件编码在  导入的数组中 检索对应的基本物料数组  D('ProductInfo')->getRightArray($value[7]/物料编码 ,$getarry,6);  


