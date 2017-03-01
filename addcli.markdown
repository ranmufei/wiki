/index.php?app=Invoicimg&m=SaleMobile&a=addsale

JSON.stringify(data)

``` javascript
//退单数据
data[shenh_uid]:1         //审核人 (*)
data[choiceData][0][id]:2204    //型号 (*)
data[choiceData][0][name]:星期   
data[choiceData][0][format]:haha-4()
data[choiceData][0][purchasePrice]:456.00         //退货价格 (*)
data[choiceData][0][sellPrice]:456.00
data[choiceData][0][saleNum]:10
data[choiceData][0][stornNum]:1          //退货数量 (*)
data[choiceData][0][batchnum]:1        //批次数量
data[choiceData][0][unit]:596        //单位 (*)
data[choiceData][0][relation]:1     //单位换算 (*)
data[choiceData][0][is_pc]:1         //是否有批次
data[choiceData][0][batch_data][0][id]:776
data[choiceData][0][batch_data][0][intonum]:5           //出库数量
data[choiceData][0][batch_data][0][name]:20161229175310       // 批次
data[choiceData][0][batch_data][0][formatname]:haha-4    //规格
data[choiceData][0][batch_data][0][productname]:星期      //产品名称
data[choiceData][0][batch_data][0][thnum]:1                  //退货数量
data[choiceData][0][batch_data][0][is_thsale]:0
data[choiceData][0][batch_data][1][id]:775
data[choiceData][0][batch_data][1][intonum]:5               
data[choiceData][0][batch_data][1][name]:20161229175011   
data[choiceData][0][batch_data][1][formatname]:haha-4     
data[choiceData][0][batch_data][1][productname]:星期       
data[choiceData][0][batch_data][1][thnum]:1              
data[choiceData][0][batch_data][1][is_thsale]:0
data[choiceData][0][batch][0][id]:775            //退货批次的id
data[choiceData][0][batch][0][num]:1             //退货批次的数量
data[choiceData][0][xlhdata]:[]            //序列号id数组                       
data[choiceData][0][unitname]:瓶
data[choiceData][0][action]:delete
data[order]:XS-TH201711610646    //订单号 (*)
data[type]:0          //退单为0 (*)
data[ordertype]:3     //(*)
data[customval]:578            客户id (*)
data[totime]:2017-01-16      //(*)
data[mark]:                     //备注(*)
data[count_price]:456.00   //(*)
data[num]:1        //(*)
data[default4]:5358        //退货订单关联销售订单的id//(*)
data[foreign_currency]:{                  //没有就为空//(*)
		money_cr:'',//外币汇率
        money_name:'',//外币名称
        money_gw:0//外币金额
		  
}