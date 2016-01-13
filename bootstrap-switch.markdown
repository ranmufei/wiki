# Bootstrap 开关（switch）组件 bootstrap-switch/avalon.switch

## 说明
  > 1，使用效果可以查看这里[url]http://www.bootcss.com/p/bootstrap-switch/[/url]
  > 2，在html中引用 <div  ms-widget="bootstrap-swtich,$,$bootstrapSwtich"> </div>



## 配置参数说明
       $bootstrapSwtich : {
              onSwitchChange : function(event,state){  //点击切换的回调函数，event是事件，state是返回的状态， true为开，false为关
                   avalon.log(state)   
               } ,
              onInit : function(){},   //初始化的操作
              state: true,     // 开始的状态, true 为开  ，  false为关
              size: null,       //默认为normal   , large大 ,small小 ， mini最小
              disabled: false,   //禁用 ,默认关
              readonly: false,  //  只读 ，默认关
              onColor: "primary",    //可选颜色风格primary,info,success,warning,danger
              offColor: "default",   //可选颜色风格primary,info,success,warning,danger
              onText: "ON",          // 开时选中的文字
              offText: "OFF",        // 关时选中的文字
              labelText: "&nbsp;",     //开与关之间的字

      } ,


##  接口方法

| 参数名称      |    必填 | 说明  |
| :-------- | --------:| :--: |
|onInit()|否| 组件初始化  |
|onSwitchChange()|是| 点击后的回调，event是事件，state是返回的状态， true为开，false为关  |




## 案例html 


```

<div ms-controller="root">

<div class="panel panel-primary">


<div class="col-md-4">
<div class="panel panel-success">
      <div class="panel-heading">
        <h3 class="panel-title">选择供应商</h3>
      </div>
      <div class="panel-body">

        <input type="text " class="form-control " ms-widget="supplier"  placeholder="供应商 ">
      </div>
</div>
</div>
</div>
</div>


```


## 使用方法

  > 引入 Avalon组件地址 supplier/avalon.supplier

   [在线预览案列](http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget) http://www.apps.com/index.php?app=Invoicimg&m=TestApi&a=widget

``` javascript

/**
* test
* 
*/


/**
* test
* 
*/
require(['avalon'
   ,'creatclass/creatclass'
   ,'unit/unit'
   ,'formatbatch/formatbatch'
   ,'choicebatch/choicebatch'
   ,'choiceproduct/choiceproduct'
   ,'warehouse/warehouse'
   ,'createproduct/createproduct'
   ,'format/format'
   ,'choiceSerial/choiceSerial'
   ,"Prewidget/Prewidget"
   ,"selcustom/avalon.selcustom"
   ,"supplier/avalon.supplier"
   ,'author/author'
   ,'domReady!'],function(avalon){
   var classmodel=null,batchoicemodel=null,serialmodel=null,accModel=null,choice=[],batmode=[];
   var model=avalon.define({ 
   			$id:'root',
   			$classopt:{
   				onInit:function(cmodel){
   					console.log('oninit:',cmodel);
   					classmodel=cmodel;
   				},
   				callbackfun:function(){
   					avalon.log('callbackfun 被调用');
   				},
   				width:'400px',
   				height:'500px',
   				title:'测试分类管理',
   			},
            $warehouseopt:{
               width:'600px',
               height:'500px',
               title:'仓库',
               callbackfun:function(){
                  avalon.log('callbackfun 回调仓库');
               },
            },
            $unitopt:{
               width:'500px',
               height:'500px',
               title:'单位管理',
               callbackfun:function(){
                  avalon.log('callbackfun 回调单位');
               },
            },
            $createproductOpt:{
               width:'730px',
               height:'500px',
               title:'添加产品',
               callbackfun:function(){
                  avalon.log('回调了 添加产品');
               },
            },
            $formatopt:{
               width:'580px',
               height:'500px',
               title:'规格管理2',
               callbackfun:function(){
                  avalon.log('回调了 规格光临222');
               },
            },
            $choiceproductopt:{
               onInit:function(choicedata){
                  choice=choicedata;
               },
               title:'选择产品3',
               batch:true,
               callbackfun:function(){
                   var xz= choice.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
             $formatbatchopt:{
               onInit:function(choicedata){
                  batmode=choicedata;
               },
               title:'pici',
               type:0,
               callbackfun:function(){
                   var xz= batmode.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
            choicecp:function(ckid,subid){                 
                  batmode.show(ckid,subid)
            },
            $batchchoiceopt:{
               onInit:function(choicedata){
                  batchoicemodel=choicedata;
               },
               title:'批次选择',
               type:0,
               callbackfun:function(){
                   var xz= batchoicemodel.getSelected();
                    avalon.log('选择的产品：',xz);
               },
            },
            choicecp2:function(ckid,subid){                 
                  batchoicemodel.show(ckid,subid)
            },
            $serialopt:{
               onInit:function(smodel){
                   serialmodel=smodel;
               },
               title:'序列号管理',
               globle:true,
            },
            serial:function(){
                //查看序列号
               // avalon.log('serialmodel:',serialModel);
                serialmodel.show('*');
            }
            ,$accessOpt:{
               onInit:function(model){
                  accModel=model;
               }
               ,title:'产品管理权限配置'
               ,key:'InvoicimgProduct'
            }
            ,accshow:function(){
               accModel.show();
            },

            setuid:function(uid){
              accModel.show(uid);

            }

            ,selcustom:{
               sureCallback:function(data){
                  PrewidgetVM.Initdata(data[0].id);
               }
            }
            ,supplier:{
               mix:1,//单选，2多选
               owner:true,//是否查看所有
               // isparent:1 //1 判断添加产品供应商根据分类获取 ，0 采购选择供应商根据产品获取
               onInit:function(vm){
                  SupplierVM=vm;
               },
               sureCallback:function(data){
                  console.log('回调数据',data);
               }
            }

            ,


   })
   avalon.scan();


})




